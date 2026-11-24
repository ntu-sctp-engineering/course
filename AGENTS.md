# AGENTS.md

Guidance for AI agents working in this repository.

## Project brief

The existing **Cloud Engineering** course is being revamped into a new **Platform Engineering** course. This repo holds the course outlines and related curriculum material for that work.

## Repo layout

* `README.md` - repo readme
* `outline/` - course outlines, one Markdown file per course
  * `platform-engineering.md` - the new Platform Engineering outline (7 modules, 3 lessons a week, a heading, summary and table per week)
  * `cloud-engineering.md` - the current Cloud Engineering outline (3 modules, tables per module; source: "CE Cohort 12" tab of Google Sheet `1l0Kjis-lhFnDtFRzYnCA-qzrCbHY0QnmpTcE60kdnr4`)
* `MEMORY.md` - running log of decisions and context; read it at the start of a session

## Course structure

* 3 modules, with units numbered `1.x`, `2.x`, `3.x`
* Units are interleaved with `CO` (coaching) sessions, numbered across the whole course

## Outline format

Use a `#` title, then a `## Module N - Name (X weeks)` heading per module.

* **Platform Engineering** splits each module into weeks: a `### Week N` heading per week (weeks numbered continuously 1-24 across the course), a one or two sentence summary of that week's lessons, then a `Unit | Lesson | Summary` table for that week's three lessons. Weeks not yet designed say "To be designed."
* **Cloud Engineering** keeps one `Week | Unit | Lesson | Summary` table per module, with weeks restarting at 1 in each module. Coaching sessions use `CO` in the Unit column. Its Summary column is one short sentence per unit from the "Shared with Students" Google Drive folder (`1_i1UjJpbAXIbDtyjQcRlVGv45mnbDmgr`); blank where no material exists.

The Summary column is one short sentence on what the lesson teaches.

```markdown
# Platform Engineering Course Outline

## Module 1 - Name (2 weeks)

### Week 1

One or two sentences summarising the week's lessons.

| Unit | Lesson | Summary |
| ---- | ------ | ------- |
| 1.1 | Title | One short sentence on what the lesson teaches. |
| 1.2 | Title | One short sentence on what the lesson teaches. |
| 1.3 | Title | One short sentence on what the lesson teaches. |
```

## Conventions

* All changes go through a pull request, assigned to Justin (`jsstrn`) for review. Don't push to `main`.
* Keep files concise and in Markdown.
* When you make a decision or learn lasting context, add a dated entry to `MEMORY.md` in the same PR.
