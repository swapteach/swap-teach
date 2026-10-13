<!-- mirror-of: reference/README.md @ 9f3e7e261689eea75be74350c9b6f782faa2996e -->
> 🌐 English mirror of [reference/README.md](../../reference/README.md). The Chinese version is authoritative.

# Reference files

Original reference files live in [`reference/`](../../reference/). **Never modify the originals**; organized summaries go in [docs/](../docs/).

| File | Contents | Trust |
|---|---|---|
| `115-1-Database_評分規定.pdf` | Prof. Chang's slides: project requirements, schedule, grading, peer review, competition bonuses, contribution split, attendance | ✅ Official |
| `Database Systems Syllabus.pdf` | Syllabus from FJU's course outline system (printed 2026-09-12) | ✅ Official |
| `507_概述文件(教育AI組)_20261005013226.docx` | Submitted competition overview, Education AI track | ✅ Our submission |
| `507_概述文件(資訊應用組)_20261005013223.docx` | Submitted competition overview, Information Applications track | ✅ Our submission |
| `2026-09-15-第一堂課逐字稿.txt` | Speech-to-text transcript of the first lecture (the professor explains the project requirements, grading, and why past projects got X marks) | ⚠️ Unofficial, many recognition errors; summary in [docs/course/first-lecture.md](../docs/course/first-lecture.md) |
| `Comprehensive Specification & Operational Benchmark Guide- Database Systems Course Term Project.txt` | English description of the course and project | ⚠️ **Unofficial, AI-generated. Do not rely on it.** |

Text versions of the two overviews are in [docs/competition/submissions/](../docs/competition/submissions/). Summaries of the official rules are in [docs/course/](../docs/course/).

## Where the AI-generated `.txt` contradicts the official slides

`Comprehensive Specification…txt` looks like an AI-generated English write-up of the slides. It contains errors and unsupported claims:

1. **Wrong competition options.** It lists the ITSA Geek Challenge and NCPC Fu Jen preliminary as ways to satisfy the 15% external competition requirement. In the slides, the 15% comes from the ICT Innovative Services Awards or "a large competition of your choice"; ITSA and NCPC are separate **semester grade bonuses**.
2. **Incomplete competition categories.** It lists only 大會專題類 and 國際交流類, missing 指定專題類 (which the Education AI track belongs to).
3. **Missing rules.** It omits: competition scoring (5 points if not a finalist, 15 as a finalist, full 40 for a winning project, semester grade 99 for top three), −5 for not using GitHub, the contribution-split formula, the "no project, no presentation → whole group gets 49" rule, and weekly attendance.
4. **Invented content.** It explains why past projects got X marks (e.g. "Stray Animal Integration was a shallow wrapper over public APIs"). The slides only list names and X counts, with no reasons. In the first lecture the professor explained the reasons for several projects (see [first-lecture.md](../docs/course/first-lecture.md#past-projects-why-they-got-x-marks)), and they differ from the `.txt`: for the bubble-tea app 手搖達人, the `.txt` blames a lack of database complexity, while the professor said it was simply useless.
5. **Reflection report.** It calls the reflection report "strictly required"; the slides only say "if there is a results showcase → reflection report".
6. **Unverifiable details.** It names Prof. Chang as the NCPC Fu Jen team coach and gives an email address; neither appears in the slides.
