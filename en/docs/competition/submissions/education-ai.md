<!-- mirror-of: docs/competition/submissions/education-ai.md @ 4ec2e808a8c6c4417cff5d589da5143b689efe0f -->
> 🌐 English mirror of [docs/competition/submissions/education-ai.md](../../../../docs/competition/submissions/education-ai.md). **AI translation for reference only.** The Chinese text is what was actually submitted.

# Submitted overview: Education AI track (教育AI組)

> **Frozen; do not edit.** Text of the overview document submitted to the 2026 31st ICT Innovative Services Awards. Original file: `reference/507_概述文件(教育AI組)_20261005013226.docx`. The latest project overview is in [docs/project/overview.md](../../project/overview.md).

---

Attachment 1-1: System Overview Document

Number: (filled in by the organizer)

Chinese title: 換你教－校園技能交換 App

English title: SwapTeach: A Campus Skill-Exchange App

## 1. Introduction

Outside their coursework, university students often want to learn more, such as a second language, a musical instrument, video editing or programming, but cram schools and paid courses are a burden for most students. There are actually many skilled students on campus, and teaching each other is a natural way to learn; there's just no everyday way to know "who can do what, and who wants to learn what."

Even after finding someone, peer teaching runs into a few problems: someone who has a skill doesn't necessarily know how to teach it and often doesn't know where to start at the first meeting; the two people's timetables differ, so just arranging a time takes lots of back-and-forth; and nothing is recorded after teaching, so it's hard to know how much the other person actually learned.

We therefore propose SwapTeach, a campus skill-exchange app that lets students trade a skill they have for a skill they want, and uses AI for two things — "finding the right person" and "helping the teacher prepare" — so that peer teaching is easier to start and easier to keep going.

## 2. Creative description

SwapTeach's core idea is "skills for skills." We borrow the swipe-card interaction from dating apps and apply it to skill exchange: each user has a skill card stating "what I can do" and "what I want to learn." Swiping right means you want to learn from the other person, swiping left means skip, and it's a match only when both swipe right.

One-to-one swaps alone often run into "I want to learn yours, but you don't want to learn mine," so we designed two mechanisms:

(1) Circular matching: when two people's skills can't be swapped directly, the system looks for a third person or more, forming a cycle where A teaches B, B teaches C and C teaches A, so everyone both teaches and learns.

(2) Time coins: teaching someone for one hour earns one time coin, which can later be used to learn from anyone for one hour, not just the same person. Whether teaching programming or baking, everyone's hour is worth the same.

AI in this system plays the role of supporting peer teaching, mainly in three places:

(1) Matching: recommends people based on skill fit, level gap and common free periods, and finds circular matching combinations.

(2) Lesson preparation: based on the learner's level, goals and planned number of meetings, generates a teaching outline and practice suggestions for each meeting, so classmates with no teaching experience have something to work from.

(3) Post-session review: based on short notes both sides fill in after a session, summarizes the key points and generates a few practice questions, helping the learner review and letting the teacher know where to pick up next time.

## 3. System features

(1) Personal skill card: enter skills you can teach, skills you want to learn, level and available times.

(2) Swipe matching: swipe left to skip, right to learn; chat opens only after both swipe right.

(3) Chat and booking: after matching, discuss what to teach and book a time and place to meet.

(4) Automatic free-period scheduling: after users import their timetables, the system automatically finds both sides' common free periods.

(5) AI learning plan: based on the learning goal and planned number of meetings, generates a teaching outline for each meeting for the teacher to reference and edit.

(6) AI post-session review: based on the notes both sides fill in after a session, generates a summary and practice questions.

(7) Time coins and circular matching: records each user's teaching and learning hours and supports multi-person cyclic exchange.

(8) Mutual rating and skill badges: users rate each other after each exchange; accumulated teaching hours earn badges; records can be exported as a personal learning portfolio.

(9) On-campus venue suggestions and saved list: suggests public places such as library discussion rooms; skill cards you're interested in but haven't decided on can be saved first.

## 4. System highlights

(1) AI helps the teacher prepare: students aren't teachers, so the system provides a teaching outline as a starting point, lowering the "I don't know how to teach" barrier.

(2) AI assists rather than replaces: learning plans and practice questions are only drafts; the teaching student can edit them, and they're given to the learner only after confirmation. Actual teaching still happens person to person.

(3) Easier to match: circular matching and time coins mean skills don't have to pair up exactly for an exchange to happen.

(4) No money needed: exchanges use skills or time coins, so students pay no tuition.

(5) Learning by teaching: teaching others is also a chance to consolidate what you know; teaching hours, badges and ratings can be exported as a learning portfolio.

(6) Campus-only with careful data use: identity is verified by school email; timetables are used only to compute common free periods; content sent to the language model excludes personal data such as names and student IDs.

## 5. Development tools and technologies

This project is currently in the planning stage. We plan to use:

(1) Frontend: Flutter, supporting both Android and iOS from one codebase.

(2) Backend and database: Python FastAPI for the API; PostgreSQL to store skill cards, match records, ratings and the time coin ledger.

(3) Matching algorithm: users are nodes, and "A's skill is exactly what B wants to learn" is a directed edge; short cycles in the graph are candidates for circular matching. General recommendations are ranked by skill fit, number of common free periods and past ratings.

(4) Language model: a large language model API. For learning plans, the input is the skill name, the learner's self-assessed level, learning goal and number of meetings, and the output is each meeting's topic and practice suggestions. For post-session reviews, the input is both sides' session notes, and the output is a summary and practice questions.

(5) Push notifications: Firebase Cloud Messaging, for successful matches and booking reminders.

(6) Data sources: user-entered skill cards, ratings and session notes; user-imported timetables; and the school's public venue information.

## 6. Target users

(1) Undergraduates: want to learn new skills but have a limited budget.

(2) Graduate students: want someone to practice a language with, or tools used in research.

(3) Clubs and student associations: need students with specific skills, such as graphic design, video editing or event hosting.

## 7. Operating environment

(1) Hardware: Android or iOS smartphone.

(2) Network: matching, chat and push notifications all require an internet connection.

(3) Account: must register and verify with a school email before use.

(4) Server: backend API and database planned for deployment on a cloud host.

## 8. Conclusion

SwapTeach addresses an everyday problem: wanting to learn something but not wanting to, or not being able to, spend much money, while there are people nearby who could teach. We believe AI in education doesn't have to be the teacher; it can also help classmates teach each other: helping find the right person, helping the teacher prepare content, and helping the learner review.

Next, we plan to first build an app prototype with swipe matching, chat and booking, then add AI learning plans and post-session reviews, pilot it on a single campus and gather feedback to confirm whether AI-generated content actually helps students, and then evaluate expanding to other schools.
