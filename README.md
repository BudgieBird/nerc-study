<p align="center">
  <h1 align="center">NERC RC Exam Study System</h1>
  <p align="center">
    An adaptive study environment for the NERC System Operator Certification Exam<br />
    (Reliability Coordinator level) built on Claude Code.<br />
    No application code — just structured reference files, AI-powered skills,<br />
    and progress tracking that work together as a personalized tutoring system.
  </p>
</p>

> [!IMPORTANT]
> This system requires [Claude Code](https://claude.ai/code) to function. The skills and commands are Claude Code primitives — they do not run as standalone scripts or applications.

<p align="center">
  <a href="https://github.com/BudgieBird/nerc-study/issues"><img alt="GitHub Issues" src="https://img.shields.io/github/issues/BudgieBird/nerc-study?color=0088ff" /></a>
  <a href="https://github.com/BudgieBird/nerc-study/pulls"><img alt="GitHub Pull Requests" src="https://img.shields.io/github/issues-pr/BudgieBird/nerc-study?color=0088ff" /></a>
  <a href="https://github.com/BudgieBird/nerc-study/graphs/contributors"><img alt="GitHub Contributors" src="https://img.shields.io/github/contributors/BudgieBird/nerc-study" /></a>
  <a href="https://github.com/BudgieBird/nerc-study/commits/main"><img alt="Last Commit" src="https://img.shields.io/github/last-commit/BudgieBird/nerc-study" /></a>
</p>

<p align="center">
  <a href="https://github.com/BudgieBird/nerc-study/releases">Releases</a>
  &middot;
  <a href="https://github.com/BudgieBird/nerc-study/issues/new">Report Bug</a>
  &middot;
  <a href="https://github.com/BudgieBird/nerc-study/issues/new">Request Feature</a>
</p>

---

## Table of Contents

- [About](#about)
- [How It Works](#how-it-works)
- [Project Structure](#project-structure)
- [Commands](#commands)
- [Skills](#skills)
- [Reference Files](#reference-files)
- [Daily Workflow](#daily-workflow)
- [Study Phases](#study-phases)
- [Getting Started](#getting-started)
- [Customization](#customization)
- [Exam Overview](#exam-overview)
- [Limitations](#limitations)
- [Contributing](#contributing)

---

## About

The NERC Reliability Coordinator (RC) certification exam tests your ability to make real-time decisions about bulk electric system reliability. It covers power system fundamentals, NERC standards, emergency procedures, and operational communications.

This system uses schema theory to map NERC concepts onto your existing professional knowledge through targeted analogies, then drills you on the specific standards, thresholds, and entity responsibilities that appear on the exam.

The entire system runs inside Claude Code. There is no web app, no database, no build step. You clone the repo, customize your profile, and start studying.

## How It Works

```
/reference/*.md  <--  ground truth (skills READ these before every response)
       ^
       |  /promote (human review gate)
       |
/reference/pending-review.md  <--  staged additions (skills WRITE here)
       ^
       |
  Skills (tutor, research, validator)
       |
       v
/progress/*.md   <--  quiz scores and weekly reviews (exam skill appends here)
```

**Skills** are Claude Code AI agents, each with a specific role and assigned model. **Commands** are slash-command wrappers that activate skills with user arguments. **Reference files** are the single source of truth -- when Claude's training data conflicts with a reference file, the file wins.

Skills never write directly to reference files. New definitions, exam traps, and standard references discovered during sessions are staged in `reference/pending-review.md` with source attribution. You review and promote staged entries to the authoritative files via `/promote`.

The exam skill reads your past scores from `/progress/daily-scores.md` and weights future question sets toward your weak domains. Missed concepts are tracked in `/progress/review-schedule.md` with spaced repetition intervals (1d, 3d, 7d, 14d, 30d) so they resurface at optimal review times. The `/review` command analyzes score trends, lists concepts due for review, compares study time distribution against official exam domain weights, and adjusts your study plan.

## Project Structure

```
nerc-study/
|
|-- .claude/
|   |-- commands/                    # Slash command definitions
|   |   |-- study.md                 #   /study [topic]
|   |   |-- quiz.md                  #   /quiz [topic|20|full]
|   |   |-- research.md              #   /research [topic]
|   |   |-- validate.md              #   /validate [claim]
|   |   |-- rapid-fire.md            #   /rapid-fire [topic]
|   |   |-- promote.md               #   /promote (review staged additions)
|   |   +-- review.md                #   /review
|   |
|   +-- skills/                      # Claude AI skill implementations
|       |-- nerc-tutor/              #   Schema-based teaching (Opus)
|       |-- nerc-exam/               #   Question generation + grading (Haiku)
|       |-- nerc-research/           #   Web search deep dives (Sonnet)
|       |-- nerc-comprehension/      #   Socratic probing (Sonnet)
|       +-- nerc-validator/          #   Fact-checking against references (Opus)
|
|-- reference/                       # Ground truth -- authoritative NERC content
|   |-- nerc-glossary.md             #   NERC definitions and key terms
|   |-- nerc-standards-map.md        #   Standards with requirements and exam focus
|   |-- exam-traps.md                #   Known exam traps and misconceptions
|   |-- analogy-map.md.example       #   Template for background-specific analogies
|   |-- frameworks-map.md            #   (if added) Regulatory framework mappings
|   +-- pending-review.md            #   Staged additions awaiting /promote review
|
|-- progress/                        # Performance tracking (auto-populated)
|   |-- daily-scores.md.example      #   Template for quiz/exam score logging
|   |-- weekly-reviews.md.example    #   Template for weekly analysis
|   +-- review-schedule.md.example   #   Template for spaced repetition tracking
|
|-- CLAUDE.md.example                # Template -- copy to CLAUDE.md and customize
+-- .gitignore                       # Keeps personal files out of version control
```

> [!NOTE]
> Files ending in `.example` are templates. The actual `CLAUDE.md`, `reference/analogy-map.md`,
> and `progress/*.md` files are in `.gitignore` so your personal data never gets committed.
> See [Getting Started](#getting-started) for setup.

## Commands

| Command | Purpose | Typical Duration |
|---|---|---|
| `/study [topic]` | Start a tutor session with 4-part format: definition, analogy, scenario, comprehension check | 45-60 min |
| `/research [topic]` | Deep-dive research using web search; stages findings for review | 15 min |
| `/quiz [topic\|20\|full]` | Generate practice exam questions, grade, and log scores | 20 min |
| `/rapid-fire [topic]` | Quick recall drilling on definitions, thresholds, and entity responsibilities | 10 min |
| `/validate [claim]` | Fact-check a claim against reference files | As needed |
| `/promote` | Review and promote staged additions to reference files | As needed |
| `/review` | Analyze scores, list spaced repetition items due, compare domain weight coverage, adjust plan | Weekly |

The comprehension skill is triggered conversationally by saying **"Challenge me on [concept]"** rather than a slash command.

## Skills

Each skill runs on a specific model chosen for the task:

| Skill | Model | Role |
|---|---|---|
| `nerc-tutor` | Opus 4.6 | Schema-based teaching with analogies mapped to student background |
| `nerc-research` | Sonnet 4.6 | Web search research on NERC standards and materials |
| `nerc-comprehension` | Sonnet 4.6 | Socratic questioning to verify deep understanding |
| `nerc-exam` | Haiku 4.5 | Fast practice question generation and grading |
| `nerc-validator` | Opus 4.6 | Independent fact-checking against reference files |

**Why different models?** Opus handles nuanced teaching and validation where accuracy is critical. Sonnet handles research and comprehension probing. Haiku handles high-volume question generation where speed matters more than depth.

## Reference Files

All files in `/reference/` are **authoritative**. Skills read these before responding, and when Claude's training data conflicts with a reference file, the reference file wins.

| File | Contents | Tracked |
|---|---|---|
| `nerc-glossary.md` | NERC definitions and key terms for the RC exam | Yes |
| `nerc-standards-map.md` | NERC standards with requirements and exam focus areas | Yes |
| `exam-traps.md` | Known exam traps and common misconceptions | Yes |
| `analogy-map.md` | Analogy mappings for all 6 exam domains, customized to student background | No (personal) |

Skills that discover new definitions, traps, or standard references during sessions stage them in `reference/pending-review.md` with source attribution. Use `/promote` to review and move approved content into the authoritative files.

## Daily Workflow

```
STEP 1 -- RESEARCH (15 min)
  /research [NERC standard or topic]
  Stages findings in pending-review.md for your review

STEP 2 -- LEARN (45-60 min)
  /study [topic]
  4-part format: Definition -> Analogy -> Scenario -> Comprehension Check
  Continues until understanding is demonstrated

STEP 3 -- PROVE (15-20 min)
  "Challenge me on [concept]"
  Socratic questioning: pass and move on, or go back to tutor

STEP 4 -- TEST (20 min)
  /quiz 20
  Exam-format questions graded and logged

STEP 5 -- VALIDATE (as needed)
  /validate [claim]
  Fact-check anything that seems wrong

STEP 6 -- PROMOTE (as needed)
  /promote
  Review staged additions and promote, edit, or discard

WEEKLY:
  /review
  Analyze scores and adjust the study plan
```

## Study Phases

| Phase | Focus |
|---|---|
| Phase 1 | Power theory foundations -- voltage, real vs reactive power, power factor, frequency |
| Phase 2 | Weakest areas from exam breakdown -- targeted study on lowest-scoring domains |
| Phase 3 | Reinforce improving domains, polish strong areas, full practice exams |

The timeline adapts to your actual study duration through the `/review` command.

## Getting Started

### Prerequisites

- [Claude Code](https://claude.ai/code) (CLI, desktop app, or IDE extension)
- An Anthropic API key or Claude Pro/Max subscription

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/BudgieBird/nerc-study.git
   cd nerc-study
   ```

2. Create your personal files from the templates:
   ```bash
   cp CLAUDE.md.example CLAUDE.md
   cp reference/analogy-map.md.example reference/analogy-map.md
   cp progress/daily-scores.md.example progress/daily-scores.md
   cp progress/weekly-reviews.md.example progress/weekly-reviews.md
   cp progress/review-schedule.md.example progress/review-schedule.md
   ```

3. Edit `CLAUDE.md` and fill in the **Student Profile** section with your actual background and exam score breakdown (if you have one).

4. Edit `reference/analogy-map.md` to match your professional background. The included template shows the expected format with generic analogies -- replace them with your own.

5. Open in Claude Code:
   ```bash
   claude
   ```

6. Start studying:
   ```
   /research COM-002
   /study three-part communication
   /quiz 20
   ```

> [!TIP]
> Your personal files (`CLAUDE.md`, `reference/analogy-map.md`, `progress/*.md`) are
> gitignored. You can `git pull` to get reference file updates without overwriting your
> profile or scores.

## Customization

The system is designed to be forked and personalized. Personal files are gitignored so you can pull upstream updates without merge conflicts.

**`CLAUDE.md`** (copied from `CLAUDE.md.example`)

Your student profile. Include your exam score breakdown if you have one -- the exam skill uses domain scores to weight question sets toward your weak areas. Every skill reads this file.

**`reference/analogy-map.md`** (copied from `reference/analogy-map.md.example`)

Maps NERC concepts to analogies drawn from your professional background. The tutor skill reads this before every response. The included template shows the expected format -- replace the example analogies with your own domain knowledge.

**What NOT to customize:** The shared reference files (`nerc-glossary.md`, `nerc-standards-map.md`, `exam-traps.md`) contain exam-accurate content. These are tracked in git. Edit them only to correct inaccuracies or add new content. If you find an error, consider opening a pull request so everyone benefits.

## Exam Overview

> [!WARNING]
> Exam format details can change. Always verify against the
> [official NERC certification page](https://www.nerc.com/pa/comp/Pages/System-Operator-Certification.aspx)
> before sitting for the exam.

| Parameter | Value |
|---|---|
| Exam | NERC System Operator Certification -- Reliability Coordinator |
| Format | Computer-based, multiple choice |
| Questions | 140 (120 scored + 20 unscored experimental) |
| Time | ~3 hours |
| Passing | 92 / 120 scored questions (RC credential) |

### 6 Exam Domains

| Domain | Focus |
|---|---|
| Communications and Data | Telecom infrastructure, 3-part comms, data exchange, situational awareness |
| Transmission | Facility ratings, SOLs, power flow, thermal/voltage/stability limits |
| Contingency Analysis and Reliability | N-1/N-2 analysis, IROLs, real-time and next-day assessments |
| Emergency Response | EEA levels, RC directive authority, inter-RC coordination |
| Emergency Preparedness | Blackstart, restoration, backup control centers, training |
| Resource and Demand Balancing | ACE, frequency response, reserves, CPS1/CPS2/BAAL |

## Limitations

**Validator same-family limitation.** The validator skill runs on the same model family (Anthropic) as the tutor. When validator confidence is low (reference files insufficient), cross-validate with a non-Anthropic model or official NERC sources.

**Not a replacement for official study materials.** This system supplements -- it does not replace -- NERC's official study materials, practice exams, or employer-provided training programs.

**Practice exams include 20 unscored items.** The real exam has 140 questions (120 scored + 20 experimental). You cannot tell which are which. The practice tool does not simulate unscored items — all generated questions count toward your score.

**Reference files can become outdated.** NERC periodically updates standards and requirements. Run `/research` regularly and verify reference files against the [official NERC standards page](https://www.nerc.com/pa/Stand/Pages/default.aspx).

**Power systems are safety-critical.** This is an exam study tool, not operational guidance. Never use AI-generated content to make real-time reliability decisions.

## Contributing

Contributions are welcome -- particularly corrections to reference files, new exam traps, and improved analogy mappings for different professional backgrounds.

1. Fork the repository
2. Create a feature branch (`git checkout -b fix/update-bal-001-requirements`)
3. Commit your changes
4. Open a pull request

If you find an inaccuracy in the reference files, please [open an issue](https://github.com/BudgieBird/nerc-study/issues/new) with a link to the authoritative NERC source.

---

<p align="center">
  Built with <a href="https://claude.ai/code">Claude Code</a>
</p>
