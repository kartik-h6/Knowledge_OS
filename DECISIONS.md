# Decisions

> Why this system is built the way it is.
> Each entry records a decision, the reasoning behind it, and what it replaced.
> A living document. Git history is the complete record.

---

## How to read this file

Every entry has four parts:

- **Decision** — what was chosen.
- **Why** — the reasoning.
- **Rejected** — the alternative that was considered and set aside.
- **Source** — where the decision is recorded in the repository.

Entries are grouped by area, not strictly by date. Where a decision has a known date, it is noted.

---

## Structure of the repository

### The core documents live at the root, numbered

**Decision.** The system documents sit at the repository root, numbered `00`–`05`.
**Why.** They are read in order and referenced constantly; a root location keeps them the first thing anyone sees.
**Rejected.** A `docs/` folder. That convention is right for code projects (it is used in PMAS and e-library) but adds a layer of navigation to a repository that is only documents.
**Source.** `README.md`.

### Folder = workflow stage; Domain = topic

**Decision.** A note lives in one folder (where it is in its life) and carries one or more domain tags (what it is about).
**Why.** The two questions — "how far along is this?" and "what is this about?" — are independent, and collapsing them into one taxonomy loses one of them.
**Rejected.** Topic folders, which would have made workflow stage invisible.
**Source.** `README.md`, `03_SECOND_BRAIN_INDEX.md`.

### The domain list is defined once

**Decision.** `01_KNOWLEDGE_MAP.md` holds the single canonical domain list. Every other document refers to it; none redefines it.
**Why.** Three overlapping lists had grown up — the domains in `01`, the recurring themes in `02`, and a separate domain list in `03` — and they had begun to disagree, which makes tagging ambiguous.
**Rejected.** Maintaining a domain list in each document.
**Recorded.** 2026-10-25.

### Git history is the changelog

**Decision.** No `CHANGELOG.md`; no manual version numbers.
**Why.** For a living, single-author repository, the commit log is a more accurate and lower-maintenance record than a file kept in sync by hand.
**Rejected.** A maintained `CHANGELOG.md` and semantic version numbers.
**Source.** `README.md` (Versioning).

---

## The writing system

### Essay numbers are permanent

**Decision.** A published essay keeps its number forever.
**Why.** Numbers are a public contract; readers and posters already reference them.
**Rejected.** Renumbering #09–#20 to fit a new season design.
**Source.** `04_ESSAY_INDEX.md`.

### The public title of Book II is settled

**Decision.** Book II is published as "RETHINKING HEALTHCARE EDUCATION". "Knowledge Under Pressure" remains the working concept name.
**Why.** The published posters are the reference, not the draft.
**Rejected.** Treating the working name as the public one.
**Source.** `04_ESSAY_INDEX.md`.

---

## The building side

### The founder framework is a peer core document

**Decision.** `05_FOUNDER_FRAMEWORK.md` sits alongside the healthcare-knowledge documents as a core system document.
**Why.** The building side of the work needs its own operating system, and it is a different kind of document from the essay and knowledge-map files. It connects to them through the Building in Public domain and the `projects/` folder.
**Rejected.** Leaving the founder material as loose notes outside the numbered core.
**Recorded.** 2026-10-25.

---

## The repository as a self-introduction

### The repository introduces its author, to a person or a machine

**Decision.** `00_ABOUT.md` (narrative), `profile.json` (structured data) and `llms.txt` (machine-readable summary) are first-class documents.
**Why.** The same repository should be able to introduce its author to a human reader and to an LLM tool without the author repeating himself in each context.
**Rejected.** A single prose biography that serves neither reader well.
**Recorded.** 2026-10-25.

### A status legend is used throughout

**Decision.** Notes and projects carry `[FACT]`, `[EXPERIMENT]`, `[LESSON]` or `[FUTURE IDEA]`.
**Why.** It keeps unfinished work from reading as finished, which is the failure mode this repository most needs to avoid.
**Source.** Borrowed from `techstudyhubcore-archive`.

---

## Rejected approaches

- **Code-project hygiene files** (`CONTRIBUTING.md`, `SECURITY.md`, `.github/` templates). This is a personal knowledge repository, not a software project. (2026-10-25)
- **Renumbering published essays** to fit a season design. (see `04_ESSAY_INDEX.md`)
- **Redefining the domain list** in more than one document. (2026-10-25)
- **Manual version numbers.** (see `README.md`)
