# Profile Runbook

> What to do, why, when, and in what order.
> If a task is not in this file, it is not a routine task: decide it, do it, then add a row.

---

## How to use this file

1. Find the row that matches what just happened.
2. Open the files it names. Every input is a file, never a memory.
3. Stop when the done-condition is met.

The point is to remove guessing about process. Judgement about content stays with you.

---

## The three LinkedIn tasks, and what each can actually do

| Task | What it is | Possible |
|---|---|---|
| **A. Prepare** | Turn `profile.json` into ready-to-paste text for each profile field | Yes |
| **B. Audit** | Compare the live profile against `profile.json` and list the gaps | Yes, with the profile open |
| **C. Edit** | Change the live headline, About, Experience, Certifications | No. LinkedIn does not allow section edits from outside. You paste. |

Reading the live profile is possible. Editing it is not. Any instruction that implies otherwise is wrong.

---

## Standing rules

- One identity across every field: Pharmacy Practice postgraduate, healthcare technology learner, founder building TechStudyHub Core.
- Every claim traces to `profile.json`. If it is not there, add it there first, then to LinkedIn.
- No metric, credential or outcome that is not recorded somewhere.
- Nothing is pasted or published until you have read it once yourself.
- Dates are recorded when the thing happens, not reconstructed later.

---

## Field map: which source feeds which LinkedIn field

| LinkedIn field | Source | Status |
|---|---|---|
| Headline | `profile.json` → `headline` | Present |
| About | `profile.json` → `summary`, `00_ABOUT.md` | Present |
| Experience | `profile.json` → `experience` | Present |
| Education | `profile.json` → `education` | Present |
| Certifications | `profile.json` → `certifications` | Present, 7 entries |
| Featured | `profile.json` → `projects`, `publication`, `contact.portfolio` | Present |
| Skills | — | **Missing.** `profile.json` has `interests`, not a skills list. Add one. |

---

## The jobs

| # | Trigger (when) | Why | Open | Done when |
|---|---|---|---|---|
| 1 | A certificate or course is completed | Value decays with delay; the entry is strongest while current | `profile.json` | Both `profile.json` and LinkedIn list it with the same date |
| 2 | A role, project or internship starts or ends | The profile should describe what you do now, not what you did once | `profile.json` | The entry states what changed because of the work |
| 3 | An essay is published | The index is the record; drift starts the moment it lags | `04_ESSAY_INDEX.md`, `NOW.md` | Index status, NOW.md and the archive agree |
| 4 | A month passes | Profiles decay; the audit is cheaper than the repair | `profile.json`, live profile | No field on the live profile contradicts `profile.json` |
| 5 | You want to write a post | The series decides what, the voice file decides how | `04_ESSAY_INDEX.md`, `editorial_os/voice.md`, `02_EDITORIAL_CONSTITUTION.md` | Published, and job 3 is done |
| 6 | A comment thread turns substantive | Comments are research material, not applause | `INBOX.md` | Answered once, or logged as a question |
| 7 | You return after a gap of two weeks or more | Do not restart from memory; restart from the files | `NOW.md`, `04_ESSAY_INDEX.md` | `NOW.md` is current |
| 8 | A paper or conference lands | Unprocessed input is lost input | `templates/paper-template.md` or `templates/conference-template.md` | A note exists and names the essay it touches |
| 9 | Once a quarter | Positioning drifts without anyone noticing | `01_KNOWLEDGE_MAP.md`, `profile.json`, `04_ESSAY_INDEX.md` | The three agree on what you are building |

---

## Job detail

### 1. A certificate is completed

- Add it to `profile.json` under `certifications`: name, issuer, date, expiry if any.
- Add it to LinkedIn Licenses and Certifications with the issuer and the same date. Attach the file.
- If it supports a claim you want to make in an essay, note it in `research/`.

### 2. A role or project starts or ends

- Write the entry as an outcome, not a duty. What changed because of the work.
- Add dates. Add it to LinkedIn Experience or Projects.
- If it produced a lesson worth publishing, log one line in `INBOX.md`.

### 3. An essay is published

- Mark it published in `04_ESSAY_INDEX.md`.
- Update `NOW.md`: next essay, current season.
- Save the post text in `published/` and the poster with it.
- Note the number in the gallery list.

### 4. Monthly profile audit

- Open the live profile beside `profile.json`.
- Go field by field. For each, write one of four words: accurate, missing, outdated, confusing.
- Prepare corrected text for every field that is not accurate.
- Paste after reading. Do not batch this into a rewrite of the whole profile.

### 5. Writing a post

- Take the next essay from `04_ESSAY_INDEX.md`. If the index has no next, that is a map problem, not a writing problem.
- Run the quality test in the index before drafting.
- Draft against `editorial_os/voice.md` and the constitution.
- Publish. Then run job 3 in the same sitting.

### 6. A substantive comment

- Reply once, to the substance, not to the praise.
- If it challenges a claim, log it in `INBOX.md` as research material.
- If it produces a better question than the one in the index, record it against that essay.

### 7. Returning after a gap

- Read `NOW.md` and the index. Do not trust recall.
- Run job 4 before publishing anything.
- Resume at the next essay in the index.

### 8. A paper or conference

- Fill the template within 48 hours, or it will not be filled.
- File it in `research/` or `thinking/`.
- State whether it supports, contradicts or extends an existing essay.

### 9. Quarterly positioning check

- Read the identity sentence in `00_ABOUT.md` and `profile.json`.
- Ask whether it still describes what you actually spend time on.
- If not: change `01_KNOWLEDGE_MAP.md` first, then the profile, then the index. In that order, so the change is reasoned rather than reactive.

---

## Current state

As of 2026-11-25:

- Published: #01 to #20. Books I and II complete.
- Next: #21, drafted, not published.
- Profile: last audit date not recorded. Run job 4 before publishing #21.
- Known gap: `profile.json` has no skills list. Add one before the next audit.
- `NOW.md` had been stale by two months; corrected alongside this file.

---

## What this runbook does not do

- It does not decide your positioning.
- It does not verify that a claim is true.
- It does not edit LinkedIn.

Those three stay with you. Everything else is meant to be a row you can follow without predicting anything.
