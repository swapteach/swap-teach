<!-- mirror-of: docs/course/grading.md @ 4ec2e808a8c6c4417cff5d589da5143b689efe0f -->
> 🌐 English mirror of [docs/course/grading.md](../../../docs/course/grading.md). The Chinese version is authoritative.

# Grading

Source: the official slides `reference/115-1-Database_評分規定.pdf`.

## Semester grade

| Component | Weight |
|---|---|
| Term project | **40%** |
| Midterm exam | 30% |
| Final exam | 30% |

**A group that builds nothing and doesn't present gets a semester grade of 49, regardless of exam scores.**

## The 40% term project

| Part | Weight | Date | What |
|---|---|---|---|
| Midterm proposal | 5% | 2026-11-10 (one week after midterms) | Confirm the topic; slides (be creative) + oral presentation |
| Final oral exam | 20% | 2026-12-22 (one week before finals) | In-class demo + oral defense |
| External competition | 15% | — | See below |

**⚠️ To confirm:** slide 6 gives the competition 15%; slide 7 says "national competition (20%)". Since 5% + 20% + 15% = 40%, 15% is the more likely figure.

## External competition scoring

Eligible competitions: (1) the 2026 31st ICT Innovative Services Awards (registration deadline 10/3), or (2) a large on- or off-campus competition of your choice. Our registration is in [docs/competition/](../competition/ict-2026.md).

| Result | Points |
|---|---|
| Not using GitHub | **−5** |
| Entered, not a finalist | 5 |
| Finalist (withdrawing counts as not a finalist) | 15 |
| Award | Term project gets full 40 points |
| Top-three award | **Semester grade set to 99** |

## Peer review (applies to both the midterm proposal and the final presentation)

**Score = 100 × (1 − total X marks received ÷ number of evaluators)**

- Presentation order is drawn by lot; classmates elect a host (the host gets +1 semester point).
- Everyone must evaluate, filling in and handing in their sheet on the spot.
- The professor only listens: no comments, no opinions. Students may ask questions but must not try to sway the room.
- All groups present in a single class session. **Once presentations start, no more evaluation sheets are handed out**; arriving late counts as absent.
- Bathroom breaks must be under 2 minutes; missing even one group's presentation means your sheet is confiscated and you're marked absent.
- **Absent students can't evaluate, and the X count is charged to the absent student.**
- Each evaluator must give at least 5 X marks (15 groups × 1/3 = 5); more groups means more.
- Every X needs a written reason about the presentation or the work itself ("I dislike the presenter" or "unpleasant voice" are not valid).

### Thresholds (example: 70 students, 68 evaluation sheets)

| X marks | Outcome |
|---|---|
| More than 25 | Recommended to change topic |
| More than 34 | **Must re-propose** |

### Past projects (topics and X counts from the slides)

| Group | Topic | X |
|---|---|---|
| 1 | Online video platform movie search | 8 |
| 2 | LinkAd: find ad partners | 22 |
| 3 | Store-opening guide app | 22 |
| 4 | Stray animal integration | 27 (change topic) |
| 5 | Torrent download website | 23 |
| 6 | Pet-friendly app | 13 |
| 7 | Music search software | 41 (re-propose) |
| 8 | Weight-loss planning app | 51 (re-propose) |
| 9 | codzy online self-learning | 8 |
| 10 | Bubble-tea master (手搖達人) | 58 (re-propose) |
| 11 | Chalish (challenge + english) | 1 |
| 12 | Rental analysis system 租哥孔明 | 0 |
| 13 | Medicine lookup | 30 (change topic) |
| 14 | Music editing software | 13 |
| 15 | Dream lover simulator | 6 |

## Contribution split within the group

The group score is split among members by peer-assessed contribution. Each member fills in one column, giving every member (including themselves) a share; shares sum to 1.

- **Adjustment:** for member i, X_i = (average share given to i by all members) − 1/(group size)
- **Individual score:** group score × (1 + X_i)
- The slides also say "below 0.01 → evaluation removed". ⚠️ Meaning to confirm.

Example (4 members, group score 70): C receives 0.3, 0.25, 0.2, 0.3; average 0.2625; X = 0.0125; score = 70 × 1.0125 ≈ 71.

Special cases in the slides:

| Case | Result |
|---|---|
| Everyone gives 0.25 | Everyone gets the group score |
| Everyone gives only themselves 1 | Whole group gets 0 ("nonsense") |
| All zeros | Whole group gets 0 |
| Two cliques giving only to each other | Group score halved ("messing around") |

## Programming contest bonuses (added to the semester grade)

| Contest | Bonus |
|---|---|
| ITSA Geek Challenge preliminary (1–3 people, 10/3 13:00–16:00) | +3 |
| NCPC Fu Jen preliminary, AY115 (3 people, 10/3 13:00–16:00) | +3 for entering; +2 more for top 6 at Fu Jen (advance to finals) |
| NCPC finals, AY115 | Top 30: +20; 31st–40th: +10 |
| 2026 Taichung regional | +3 for entering; silver or better +20; bronze +10 |

The ITSA and NCPC preliminaries ran at the same time, so you could only pick one; both took place on 10/3.
