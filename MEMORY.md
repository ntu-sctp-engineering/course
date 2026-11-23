# MEMORY.md

Running log of decisions and context for future sessions. Add new entries at the top of the log, dated `YYYY-MM-DD`.

## Context

* Goal: revamp the Cloud Engineering course into a new Platform Engineering course.
* The Cloud Engineering outline is in `course/outline/cloud-engineering.md`, built from the "CE Cohort 12" tab of Google Sheet `1l0Kjis-lhFnDtFRzYnCA-qzrCbHY0QnmpTcE60kdnr4`.
* The course has 3 modules (units `1.x`, `2.x`, `3.x`) plus `CO` coaching sessions.

## Log

* 2026-11-23 - Filled Platform Engineering Module 1 (Cloud Computing Foundations) lessons 1.1-1.6 and added a `Summary` column to every Platform Engineering table (blank for units not yet designed), at Justin's request. Lessons: Introduction to Cloud Computing, Linux Essentials, Networking Essentials, Cloud Security and Identity, Cloud Networking with VPC, Compute in the Cloud. Cut from Cloud Engineering Module 1: Windows servers (Linux only), the OSI model in depth, RAID, High Availability & DR, Load Balancing, Database I/II (HA, load balancing and databases left for M2 architecture), and Cloud Migration. Servers Administration I/II merged into Linux Essentials, Networking Essentials and Network Communications Protocol merged into one lesson. IAM basics now sit in M1, so M2 should cover IAM through Terraform rather than reintroduce it.

* 2026-11-23 - Platform Engineering module titles now use title case (acronyms such as IaC, AI and DevSecOps kept as is), M1 renamed from "Cloud computing fundamentals" to "Cloud Computing Foundations", and unit 7.3 changed from Project Consultation to Guest Speaker, at Justin's request. Capstone is now 7.1, 7.2, 7.4, 7.5 Project Consultation, 7.3 Guest Speaker, 7.6 Project Presentation.

* 2026-11-23 - Added a `Summary` column to every table in `course/outline/cloud-engineering.md`, at Justin's request: one short sentence per unit, taken from the lesson slides (lessons) or activity docs (coaching) in the "Shared with Students" Drive folder `1_i1UjJpbAXIbDtyjQcRlVGv45mnbDmgr`. Coaching rows were summarised too, since Justin asked for all units. No material exists for 3.16 Case Study & Capstone Prep, Coaching 15 or Coaching 23, so those cells are blank.
* 2026-11-23 - Platform Engineering weeks now run continuously across the course (M1 1-2, M2 3-6, M3 7-10, M4 11-14, M5 15-18, M6 19-22, M7 23-24) instead of restarting per module, at Justin's request. Unit numbers unchanged. Cloud Engineering still restarts weeks per module.
* 2026-11-23 - Renamed the outline table column from "Lesson title" to "Lesson" in both outlines and AGENTS.md, at Justin's request. Filled in Platform Engineering capstone: 7.1-7.5 Project Consultation, 7.6 Project Presentation.
* 2026-11-23 - Converted `course/outline/cloud-engineering.md` from bullets to a Week / Unit / Lesson title table per module, because Justin wants outlines in table format. Module names and weeks come from the sheet; weeks restart at 1 in each module (sheet weeks 1-6, 7-16, 17-24). Module 2 weeks 9-10 are coaching only (cloud certification self-study weeks).
* Preference: Justin wants all course outlines as tables (Week / Unit / Lesson, one per module), not bullet lists.
* 2026-11-23 - Added `course/outline/platform-engineering.md` skeleton: 7 modules (2+4+4+4+4+4+2 = 24 weeks), 3 lessons a week, units numbered within each module (1.1-1.6 ... 7.1-7.6), 72 units in all. Lesson titles left blank for now. Weeks restart at 1 in each module. Uses a Week / Unit / Lesson title table per module instead of bullets, because Justin asked for an "outline table".
* 2026-11-23 - Added `AGENTS.md` and `MEMORY.md` to give agents the brief, layout and conventions.
* 2026-11-23 - Cloud Engineering outline merged in PR #1.
* Convention: all repo changes go through PRs assigned to Justin.
