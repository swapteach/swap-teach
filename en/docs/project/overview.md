<!-- mirror-of: docs/project/overview.md @ 4ec2e808a8c6c4417cff5d589da5143b689efe0f -->
> 🌐 English mirror of [docs/project/overview.md](../../../docs/project/overview.md). The Chinese version is authoritative.

# Project overview: SwapTeach 換你教 – Campus Skill-Exchange App

This is the **latest** project overview. It's based on the submitted Education AI track (教育AI組) overview and is updated as the project changes. The original submitted versions are in [docs/competition/submissions/](../competition/submissions/). Terms are defined in [CONTEXT.md](../../../CONTEXT.md).

## The problem

- University students want to learn skills outside their coursework (a second language, an instrument, video editing, programming…), but cram schools and paid courses are expensive.
- Plenty of students on campus have skills to share, but there's no way to know "who can do what, and who wants to learn what". Posting on social media for a skill swap gets buried quickly, and you can't see the other person's Level or availability.
- Even when two students find each other, peer teaching runs into three problems:
  1. Someone who has a skill doesn't necessarily know how to teach it, or where to start in the first Session.
  2. Their Timetables differ, so arranging a time takes lots of back-and-forth.
  3. Nothing is recorded afterwards, so it's hard to tell how much the Learner actually learned.

## Core idea: trade skills for skills

- Every User has a **Skill Card** listing Offered Skills and Wanted Skills.
- Borrowing the **Swipe** from dating apps: swipe right to want to learn from someone, left to pass; a **Match** happens only when both swipe right.
- One-to-one swaps often hit "I want to learn yours, but you don't want to learn mine", so there are two extra mechanisms:
  - **Circular Match**: the system finds a third person or more to form a cycle: A teaches B, B teaches C, C teaches A.
  - **Time Coin**: teaching one hour earns one coin, which can be spent to learn one hour from anyone. Every hour is worth the same, regardless of Skill.

## Features

1. **Skill Card**: Offered Skills, Wanted Skills, Level, and availability.
2. **Swipe matching**: chat opens only after both swipe right.
3. **Chat and Booking**: after a Match, discuss what to teach and book a Session's time and place.
4. **Automatic scheduling by Common Free Period**: after importing Timetables, the system finds when both users are free.
5. **AI Lesson Plan**: from the learning goal and planned number of Sessions, generates an outline for each Session for the Teacher to use and edit.
6. **AI Session Review**: from both users' Session Notes, generates a summary and practice questions.
7. **Time Coins and Circular Match**: records each User's teaching and learning hours; supports multi-person cycles.
8. **Rating and Skill Badges**: users rate each other after a Session; accumulated teaching hours earn badges; records export as a Learning Portfolio.
9. **Campus Venue suggestions and Saved List**: suggests public places like library study rooms; Skill Cards can be saved for later.

## The role of AI

AI **supports peer teaching**; it doesn't replace it. Teaching still happens person to person.

| Use | Input | Output |
|---|---|---|
| Match recommendations | Skill fit, Level gap, Common Free Periods | Recommended users, Circular Match combinations |
| AI Lesson Plan | Skill name, Learner's self-assessed Level, learning goal, number of Sessions | Topic and practice suggestions per Session (draft; given to the Learner only after the Teacher approves) |
| AI Session Review | Both users' Session Notes | Summary and practice questions |

Content sent to the language model excludes personal data such as names and student IDs.

## Highlights

1. AI helps the Teacher prepare, lowering the "I don't know how to teach" barrier.
2. AI assists: Lesson Plans and practice questions are drafts that the Teacher can edit and must approve.
3. Circular Matches and Time Coins mean skills don't have to pair up exactly.
4. It's free.
5. Learning by teaching; teaching hours, badges and Ratings export as a Learning Portfolio.
6. Campus-only: identity verified by school email; Timetables are used only to compute Common Free Periods.

## Planned tech (not final)

| Layer | Technology |
|---|---|
| Frontend | Flutter (Android and iOS) |
| Backend | Python FastAPI |
| Database | PostgreSQL (Skill Cards, Match records, Ratings, Time Coin Ledger) |
| Matching algorithm | Users are nodes; "A's Offered Skill is B's Wanted Skill" is a directed edge; short cycles in the graph are Circular Match candidates. Regular recommendations rank by skill fit, Common Free Periods and past Ratings |
| Language model | Large language model API |
| Push notifications | Firebase Cloud Messaging (Match made, Booking reminders) |
| Deployment | Cloud host (or the department VM) |

## Users and environment

- **Users:** undergraduates, graduate students (language exchange, research tools), clubs and student associations (finding people for design, editing, hosting, etc.).
- **Hardware:** Android or iOS phone.
- **Network:** matching, chat and notifications need internet.
- **Account:** register and verify with a school email.

## Open issues

1. **⚠️ 200,000 public records.** The course requires 200,000+ records from public data, open data, or our own scraping. The data sources planned so far are user-entered Skill Cards, Ratings and Session Notes, imported Timetables, and the school's public venue info. **None of these is a 200,000-record public dataset.** We need a large public data source relevant to the project (e.g. course data, skill taxonomies, learning resources) and an explanation of how the system uses it.
2. **⚠️ Programming language.** The syllabus says Java on Android; we plan Flutter and Python. Need to confirm with the professor.
3. **Terms to clarify.** See the "Open questions" section at the end of [CONTEXT.md](../../../CONTEXT.md).

## Next steps

1. Build an app prototype with Swipe matching, chat and Booking.
2. Add AI Lesson Plan and AI Session Review.
3. Pilot on one campus and gather feedback, checking whether the AI-generated content actually helps.
4. Evaluate expanding to other schools.
