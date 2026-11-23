# AGENTS.md

Guidance for AI agents working in this repository.

## Project brief

The existing **Cloud Engineering** course is being revamped into a new **Platform Engineering** course. This repo holds the course outlines and related curriculum material for that work.

## Repo layout

* `README.md` - repo readme
* `outline/` - course outlines, one Markdown file per course
  * `platform-engineering.md` - the new Platform Engineering outline (7 modules, 3 lessons a week, tables per module)
  * `cloud-engineering.md` - the current Cloud Engineering outline (3 modules, tables per module; source: "CE Cohort 12" tab of Google Sheet `1l0Kjis-lhFnDtFRzYnCA-qzrCbHY0QnmpTcE60kdnr4`)
* `MEMORY.md` - running log of decisions and context; read it at the start of a session

## Course structure

* 3 modules, with units numbered `1.x`, `2.x`, `3.x`
* Units are interleaved with `CO` (coaching) sessions, numbered across the whole course

## Outline format

Use a `#` title, then one table per module under a `## Module N - Name (X weeks)` heading. Platform Engineering numbers weeks continuously across the course (1-24); the Cloud Engineering outline restarts weeks at 1 in each module. Coaching sessions use `CO` in the Unit column. The Cloud Engineering outline also has a fourth `Summary` column: one short sentence per unit, summarising its lesson material from the "Shared with Students" Google Drive folder (`1_i1UjJpbAXIbDtyjQcRlVGv45mnbDmgr`); leave it blank where no material exists.

```markdown
# Platform Engineering Course Outline

## Module 1 - Name (2 weeks)

| Week | Unit | Lesson | Summary |
| ---- | ---- | ------ | ------- |
| 1 | 1.1 | Title | One short sentence on what the lesson teaches. |
| 1 | 1.2 | Title | One short sentence on what the lesson teaches. |
| 1 | CO | Coaching 1 | One short sentence on what the session covers. |
```

## Conventions

* All changes go through a pull request, assigned to Justin (`jsstrn`) for review. Don't push to `main`.
* Keep files concise and in Markdown.
* When you make a decision or learn lasting context, add a dated entry to `MEMORY.md` in the same PR.
