<!-- mirror-of: docs/course/first-lecture.md @ 9f3e7e261689eea75be74350c9b6f782faa2996e -->
> 🌐 English mirror of [docs/course/first-lecture.md](../../../docs/course/first-lecture.md). The Chinese version is authoritative.

# First lecture notes (2026-09-15)

Source: [`reference/2026-09-15-第一堂課逐字稿.txt`](../../../reference/2026-09-15-第一堂課逐字稿.txt), a speech-to-text transcript of the first lecture.

> ⚠️ The transcript comes from automatic speech recognition, has many errors, and **is not an official document**. The official slides and syllabus win. This page only adds what the slides don't say, or what helps explain them. Anything that disagrees with the slides is marked "⚠️ To confirm".

The official rules are summarized in [requirements.md](requirements.md) and [grading.md](grading.md).

## Project requirements

- **An app is preferred.** The professor prefers an app (Android resources are easier to find). For a competition you can skip the app, but you have to explain why that's more creative than an app; **"I want to build a website" with no reason is not accepted**, because websites are too easy to copy from ready-made templates.
- **Check whether it's been done.** Before choosing a topic, research what others have built and how far they went. If someone has already built it, just use theirs; there's no need to rebuild it.
- **AI can be someone else's.** Writing your own AI or using someone else's (e.g. calling an API) are both fine; the point is to build something interesting on top of it. He wants more creativity and thinks most past topics weren't put together with much care.
- **Data must be obtained legally.** Your own scraping, government open data, or other sources are all fine, as long as it's legal.
- **The dataset has to be large.** His reasoning: with only one or two hundred records you'd just use a file; you wouldn't need a database. ⚠️ To confirm: the transcript says "2.2 million fields" (220 萬個欄位), while the slides say "200,000 records". It may be a recognition error, or a difference between "fields" and "records".
- **Networked.** A standalone app doesn't have enough capacity, and the AI runs remotely anyway.
- **Servers.** The department VM has a public IP (140.136.x.x) reachable from home; free cloud services are also fine if you explain your setup.
- **GitHub.** At the end you give the professor the repo URL. If the code truly can't be public, you can host it privately (e.g. on a NAS).
- **Number of groups.** He wants no more than 15 groups (the department has about 30 tablets and 30 VMs). ⚠️ To confirm: the transcript says something like "if you want three (people), I'll grade at 90%", meaning unclear.
- **Language.** He said the Android textbook doesn't have to be the listed edition, "anything you can get started with is OK", and didn't require Java. ⚠️ Still need to confirm Flutter is accepted.

## Midterm and final presentations

- **The midterm presentation is a progress report.** The start-of-term proposal moved to the week after the midterm exam, giving everyone the first half of the term to settle on a topic.
- **Classmates grade; the professor doesn't.** He stays silent during presentations so nobody can say he's swaying the room.
- **Three criteria: completeness, creativity, usability** (完整度、創意、可用). He has each scored separately.
- **An X needs a valid reason.** Accepted examples: the UI isn't good-looking, low usability, wrong database record count, not using GitHub, **no visible database design process**. Not accepted: disliking the presenter, having a grudge.
- **No canvassing or colluding.** E.g. asking others "don't give us X"; those X marks go onto the colluders' own group.
- **"Corpses" aren't evaluated.** A group with no product at the presentation, or whose demo crashes or spins forever, is a "corpse" (屍體), and he asks the class not to evaluate it. With no product, you won't pass no matter how well you did on the exams.
- **If you've already reached a competition final or won before the presentation, say so**, so classmates know.

## Past projects: why they got X marks

| Project | X | The professor's explanation |
|---|---|---|
| Chalish (English training app) | 1 | Fewest X |
| Rental analysis system 租哥孔明 | 0 | **Very complete**: enter a location, it finds nearby rentals and scores them with its own criteria (how many meters to a 7-Eleven, gas station, and other amenities), and it even included government soil-liquefaction data |
| Dream lover simulator | 6 | Draw your ideal partner and it blends many photos into one face. The results were a bit odd, and one classmate said they can't draw so it's useless to them, but **the professor considered it very creative** |
| Bubble-tea master 手搖達人 | 58 | **Useless**: you only ever buy from a few shops; nobody needs an app to find the best one |
| Weight-loss planner | 51 | **Overpromised**: the pitch said a photo would give you the calories, so it scored well at the midterm; in the final product every bowl of beef noodles was 250 kcal. The photo was a gimmick; it was just a lookup |
| Music search software | 41 | **Copying**: KKBOX and similar services already do this well |
| Online video platform movie search | 8 | Many similar services exist, so it was unlikely to be rated highly |
| Medicine lookup | 30 | **Nobody would trust it**: no one on the team was a pharmacist, and classmates worried "who's responsible if it kills me?" |

## External competition

- **15% vs 20% explained.** He said it used to be "20% here, 15% there"; since only 1 of 16 groups reached the final last time, he moved 5% into peer review. So: **final presentation 20%, external competition 15%**.
- **Without entering any competition, the term project maxes out at 85** (you lose those 15 of the 40 points).
- You must enter one competition this term, on or off campus, but on-campus competitions earn fewer points.
- Reaching the final depends on picking the right track.
- Top three in a **large national competition**: semester grade 99 even with zero on both exams. Winning an award in a smaller competition: full 40 points for the term project.
- Last year's finalist group rehearsed with him three times before presenting at the final.

## Contribution split

- He has seen someone given 0.001; **that person is treated as having done nothing and gets 0 for the term project**. (This matches the slide's "below 0.01 → evaluation removed".)
- The contribution split must not be used to threaten teammates.
- If one person gets very low shares from all three teammates, he assumes there's probably a real problem; if someone says "the other three ganged up and gave me 0", he'll ask those three why.
- "Two cliques giving only to each other → score halved" was a joke and has never happened.
- If someone pays another person to do their project, you can report it anonymously and he'll investigate.

## Other

- Lectures are recorded and streamed, but not so you can skip class.
- No homework, because past homework got copied around.
- He gives past exam papers, but not the answers.
- Programming-contest bonuses are **added after** the semester grade is computed, not rescaled; the highest grade he gives is 99 or 100.
- ⚠️ To confirm: he said ITSA registration closed on 9/11 ("18 was my typo"), with the contest that Saturday; the [timeline](timeline.md) currently says registration closed 9/18 and the contest was 10/3, based on the slides.
