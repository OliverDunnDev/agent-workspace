# Learning Workflow Plan

**Status:** Draft, awaiting approval
**Date:** 2026-10-07

## Purpose

A repeatable workflow where you give me a topic and I run an intake interview (why, goals, timeframe), sanity-check the topic against your goals, propose a plan for approval, then build a dedicated learning pack of concept sheets and resources.

**Analogy:** a personal trainer's intake. They ask why you're there, what you're aiming for and how long you've got. Then they build the program, and they'll say so if your goal and your plan don't match.

## The 6 stages

### Stage 1: Intake
You give me a topic. I ask in small batches (3-4 questions at a time):
- **Why:** job requirement, curiosity, a project, a promotion, a career pivot?
- **Goal:** what should you be able to *do* afterwards? (explain it, build it, pass an interview)
- **Timeframe:** overall deadline and hours per week
- **Starting point:** what you already know, and how you like to learn (reading, building, video)

### Stage 2: Reality check
I compare your answers with the topic. If they don't line up, I suggest better-fitting alternatives and explain why. You decide, and I never override you.

### Stage 3: Proposed plan (approval gate)
A short plan containing:
- Refined goal in one sentence
- Roadmap in phases, scaled to your timeframe
- List of sheets I'll build
- Time estimate per phase
- What is deliberately left out, and why

**Nothing is built until you approve.**

### Stage 4: Build the learning pack
One folder per topic:

```
/guides/<topic>/
  00-roadmap.md         Phases, milestones, timeline
  01-concepts.md        Digestible concepts, each with an analogy
  02-resources.md       Curated links/docs/videos, ranked "start here"
  03-practice.md        Hands-on exercises matched to your goal
  04-cheatsheet.md      One-page quick reference
  05-progress-check.md  Self-quiz and "what next" checklist
```

Each concept follows the same pattern: **plain-English definition, analogy, tiny example, common mistake.**

### Stage 5: Review and improve
I re-read the pack against your goal and timeframe. I check for gaps, heavy jargon and anything that won't fit your schedule, then fix weak spots.

### Stage 6: Deliver and check in
I summarise the pack and tell you where to start today. When you finish a phase, come back and I'll adjust the plan.

## Design decisions (recommended defaults)

| Decision | Recommendation |
|---|---|
| Format | Markdown files in `/guides` (simple, editable) |
| Reusable template | Save intake questions and pack structure in `/templates` |
| Automation | Run by hand first; turn it into a `/learn <topic>` command once the workflow feels right |
| Resource sourcing | Live web research for current links (slower, but more accurate in fast-moving fields) |

## Build steps once approved
1. Create `/templates/learning-intake.md` (the question bank)
2. Create `/templates/learning-pack/` (the six blank sheet templates)
3. Test the workflow end to end on one real topic of your choice
4. Refine based on how it felt, then optionally build `/learn`
