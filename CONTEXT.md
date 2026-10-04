# 換你教 SwapTeach — 名詞表 Glossary

本專案的專有名詞（中英對照）。所有文件、Issues 與討論都使用這裡的用詞；「_避免_」列出的是不要使用的說法。
Project-specific terms, Chinese and English. All docs, issues and discussions use these terms; words under _Avoid_ should not be used.

> 本檔中英並列，是唯一不分成中英兩個檔案的文件。新增名詞時，中文與英文都要填。
> This file is bilingual on purpose. When adding a term, fill in both languages.

## 人 People

**使用者 User**：
通過學校信箱驗證的在校學生。
A currently enrolled student verified by school email.
_避免 Avoid_：會員、帳號、Member, Account

**教學者 Teacher**：
在一次見面中負責教的使用者。
The user who teaches in a given Session.
_避免 Avoid_：老師、導師、Tutor, Mentor

**學習者 Learner**：
在一次見面中負責學的使用者。
The user who learns in a given Session.
_避免 Avoid_：學生、Student

## 技能 Skills

**技能 Skill**：
一項可以被教、也可以被學的能力，例如吉他、日文、Python。
An ability that can be taught and learned, e.g. guitar, Japanese, Python.

**技能卡 Skill Card**：
每位使用者的個人卡片，列出會的技能、想學的技能、程度與可配合的時段。
A user's card listing Offered Skills, Wanted Skills, Levels and availability.
_避免 Avoid_：個人檔案、名片、Profile, Card

**會的技能 Offered Skill**：
使用者願意教的技能。
A Skill the user is willing to teach.
_避免 Avoid_：專長、Expertise

**想學的技能 Wanted Skill**：
使用者想學的技能。
A Skill the user wants to learn.

**程度 Level**：
使用者對自己某項技能的自評熟練度。
A user's self-assessed proficiency in a Skill.

## 配對 Matching

**滑卡 Swipe**：
瀏覽技能卡時的操作：右滑表示想跟對方學，左滑表示略過。
The action on a Skill Card: swipe right to want to learn from them, swipe left to pass.

**配對 Match**：
兩位使用者互相右滑後成立的關係；成立後才能聊天。
The relationship formed when two users both swipe right; chat opens only after a Match.
_避免 Avoid_：媒合、Pair

**環狀配對 Circular Match**：
三人以上形成的教學循環（A 教 B、B 教 C、C 教 A），用於兩人技能無法直接互換時。
A teaching cycle of three or more users (A teaches B, B teaches C, C teaches A), used when two users can't swap directly.
_避免 Avoid_：循環交換、Loop, Ring, Cycle Swap

**收藏清單 Saved List**：
使用者先收藏、尚未決定的技能卡。
Skill Cards a user has saved for later without deciding.
_避免 Avoid_：我的最愛、Favorites

## 時間與見面 Scheduling

**見面 Session**：
教學者與學習者實際碰面進行一次教學。
One actual meeting where a Teacher teaches a Learner.
_避免 Avoid_：上課、課程、Class, Lesson, Meeting

**預約 Booking**：
為一次見面約定的時間與地點。
The agreed time and place for a Session.
_避免 Avoid_：約會、Appointment, Date

**課表 Timetable**：
使用者匯入的學校課程時間表，只用來計算共同空堂。
The class schedule a user imports, used only to compute Common Free Periods.
_避免 Avoid_：行事曆、Schedule, Calendar

**共同空堂 Common Free Period**：
兩位（或多位）使用者課表中都沒有課的時段。
A time slot when all involved users have no classes.
_避免 Avoid_：空閒時間、Free time

**校內地點 Campus Venue**：
系統建議的校內公開見面場地，例如圖書館討論室。
A public on-campus place suggested for Sessions, e.g. a library study room.

## 時間幣 Time Coins

**時間幣 Time Coin**：
教一小時得一枚、學一小時花一枚的點數；不論技能，每個人的一小時都等值。
A credit earned by teaching one hour and spent to learn one hour; every hour is worth the same regardless of Skill.
_避免 Avoid_：點數、代幣、Points, Credits, Tokens

**時間幣帳本 Time Coin Ledger**：
記錄每一筆時間幣增減的紀錄。
The record of every Time Coin earned or spent.
_避免 Avoid_：餘額表、Balance table

## AI 功能 AI Features

**AI 學習計畫 Lesson Plan**：
AI 依學習者程度、目標與預計見面次數產生的每次見面大綱草稿；教學者修改確認後才提供給學習者。
An AI-drafted outline for each Session, based on the Learner's Level, goals and planned number of Sessions; the Teacher edits and approves it before the Learner sees it.
_避免 Avoid_：課程大綱、教案、Syllabus, Curriculum

**課後紀錄 Session Notes**：
教學者與學習者在見面後各自填寫的簡短紀錄。
Short notes the Teacher and Learner each write after a Session.

**AI 課後回顧 Session Review**：
AI 依課後紀錄產生的重點整理與練習題。
An AI-generated summary and practice questions based on the Session Notes.
_避免 Avoid_：測驗、Quiz, Recap

## 評價與紀錄 Reputation

**互評 Rating**：
見面結束後雙方對彼此的評分。
The scores two users give each other after a Session.
_避免 Avoid_：評論、Review（Review 已用於 Session Review）

**技能徽章 Skill Badge**：
累積教學時數達到門檻後獲得的徽章。
A badge earned after reaching a threshold of teaching hours.

**學習歷程 Learning Portfolio**：
可匯出的個人紀錄，包含教學時數、徽章與評價。
An exportable personal record of teaching hours, badges and Ratings.

## ⚠️ 待釐清 Open questions

這些名詞在概述文件中意思不夠明確，需要組員討論後決定。
These are ambiguous in the proposal and need a team decision.

1. **交換 Exchange** 指的是什麼？整段配對關係（可能包含多次見面），還是一次見面？概述文件寫「每次交換結束後互相評分」——互評是每次見面後，還是整段關係結束後？
   What is an "Exchange"? The whole Match (possibly many Sessions), or one Session? Is Rating after every Session or at the end?
2. 環狀配對需要每個人都同意（右滑）才成立嗎？
   Does a Circular Match need every member to agree (swipe right)?
3. 一對一直接互教時，也要記錄時間幣嗎？還是只有單向教學時才用？
   Do direct one-to-one swaps also record Time Coins, or only one-way teaching?
4. 時間幣的最小單位是一小時，還是可以半小時？
   Is the smallest Time Coin unit one hour, or can it be half an hour?
5. 程度用什麼刻度（例如 1–5、初級/中級/高級）？
   What scale does Level use (e.g. 1–5, beginner/intermediate/advanced)?
6. 社團與系學會是以個人帳號使用，還是有團體帳號？
   Do clubs use individual accounts, or is there a group account?
