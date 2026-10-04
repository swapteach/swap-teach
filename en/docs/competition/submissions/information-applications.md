<!-- mirror-of: docs/competition/submissions/information-applications.md @ 4ec2e808a8c6c4417cff5d589da5143b689efe0f -->
> 🌐 English mirror of [docs/competition/submissions/information-applications.md](../../../../docs/competition/submissions/information-applications.md). **AI translation for reference only.** The Chinese text is what was actually submitted.

# Submitted overview: Information Applications track (資訊應用組)

> **Frozen; do not edit.** Text of the overview document submitted to the 2026 31st ICT Innovative Services Awards. Original file: `reference/507_概述文件(資訊應用組)_20261005013223.docx`. The latest project overview is in [docs/project/overview.md](../../project/overview.md).

---

Attachment 1-1: System Overview Document

Number: (filled in by the organizer)

Chinese title: 換你教－校園技能交換 App

English title: SwapTeach: A Campus Skill-Exchange App

## 1. Introduction

Outside their coursework, university students often want to learn more, such as a second language, a musical instrument, video editing or programming. But the cost of cram schools and paid courses is a considerable burden for most students.

At the same time, there are many skilled students on campus; there's just no everyday way to know "who can do what, and who wants to learn what." The common approach today is posting on social media to look for a skill swap, but posts are easily buried by other messages, and it's hard to tell at a glance the other person's level and available times, so it usually goes nowhere.

We therefore propose SwapTeach, a campus skill-exchange app that lets students trade a skill they have for a skill they want, connecting learning resources that are currently scattered across campus.

## 2. Creative description

SwapTeach's core idea is "skills for skills." We borrow the swipe-card interaction from dating apps and apply it to skill exchange: each user has a skill card stating "what I can do" and "what I want to learn." Swiping right means you want to learn from the other person, swiping left means skip, and it's a match only when both swipe right.

One-to-one swaps alone often run into "I want to learn yours, but you don't want to learn mine." To solve this, we designed two mechanisms:

(1) Circular matching: when two people's skills can't be swapped directly, the system looks for a third person or more, forming a cycle where A teaches B, B teaches C and C teaches A, so everyone both teaches and learns.

(2) Time coins: teaching someone for one hour earns one time coin, which can later be used to learn from anyone for one hour, not just the same person. Whether teaching programming or baking, everyone's hour is worth the same.

In addition, the system uses AI to help recommend people, arrange times and generate learning plans, reducing back-and-forth communication.

## 3. System features

(1) Personal skill card: enter skills you can teach, skills you want to learn, level and available times.

(2) Swipe matching: swipe left to skip, right to learn; chat opens only after both swipe right.

(3) Chat and booking: after matching, discuss what to teach and book a time and place to meet.

(4) Automatic free-period scheduling: after users import their timetables, the system automatically finds both sides' common free periods.

(5) AI learning plan: based on the learning goal and planned number of meetings, generates a teaching outline for each meeting for the teacher to reference and edit.

(6) Time coins and circular matching: records each user's teaching and learning hours and supports multi-person cyclic exchange.

(7) Mutual rating and skill badges: users rate each other after each exchange; accumulated teaching hours earn badges; records can be exported as a personal learning portfolio.

(8) On-campus venue suggestions: suggests public places such as library discussion rooms, making first meetings feel safer.

(9) Saved list: save skill cards you're interested in but haven't decided on yet.

## 4. System highlights

(1) No money needed: exchanges use skills or time coins, so students pay no tuition.

(2) Intuitive: swiping replaces filling in forms and reading long posts; a skill card takes seconds to read.

(3) Easier to match: circular matching and time coins mean skills don't have to pair up exactly for an exchange to happen.

(4) No back-and-forth to arrange times: the system lists common free periods directly from timetables and suggests public on-campus venues.

(5) Campus-only, more trustworthy: identity is verified by school email, plus mutual ratings after every exchange.

(6) A record of learning: teaching hours, badges and ratings can be exported as part of a personal learning portfolio.

## 5. Development tools and technologies

This project is currently in the planning stage. We plan to use:

(1) Frontend: Flutter, supporting both Android and iOS from one codebase, handling the swipe interface, chat and booking screens.

(2) Backend: Python FastAPI, providing APIs for matching, booking, time coins and more.

(3) Database: PostgreSQL, storing skill cards, match records, ratings and the time coin ledger.

(4) Matching algorithm: users are nodes, and "A's skill is exactly what B wants to learn" is a directed edge; short cycles in the graph are candidates for circular matching. General recommendations are ranked by skill fit, number of common free periods and past ratings.

(5) Language model: a large language model API, generating learning plan outlines from learning goals.

(6) Push notifications: Firebase Cloud Messaging, for successful matches and booking reminders.

(7) Data sources: user-entered skill cards and ratings, user-imported timetables, and the school's public venue information.

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

SwapTeach addresses an everyday problem: wanting to learn something but not wanting to, or not being able to, spend much money, while there are people nearby who could teach. Through swipe matching, circular matching and time coins, we hope to make skill exchange easy to start and easy to keep going.

Next, we plan to first build an app prototype with swipe matching, chat and booking, pilot it on a single campus and gather feedback, then gradually add time coins and circular matching; if it works well, we'll evaluate expanding to other schools and online teaching.
