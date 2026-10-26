# Student Profile & Onboarding — Design Brief
**Companion to:** `student-profile.html` mockup
**For:** Product & Engineering
**Status:** Mockup complete, ready for scoping

---

## 1. Objective

Almost every feature that makes aspire.world more than a listings page — personalized matching, backward-planned steps, document expiry alerts, loan eligibility, agency pre-qualification — depends on the platform actually knowing something about the student. A thin profile means a thin product; this page is our answer to "what exactly do we need to know, and why."

Two principles shaped every field in the mockup:

- **Nothing is collected without a reason a student can see.** Each section below is labeled with what it powers, matching the tags shown in the mockup itself (Required at signup / Powers matching / Optional).
- **We ask progressively, not all at once.** The mockup shows the *full* profile for engineering's reference — but the real onboarding flow should not force all of this in one sitting. See the staged approach below.

---

## 2. The staged approach — what we ask, and when

Forcing a 30-field form at signup kills conversion before a student ever sees the product's value. Instead, profile completion should unlock progressively, the same way the Finance panel already unlocks contextually in the dashboard.

| Stage | When | Fields requested | What it unlocks |
|---|---|---|---|
| **1 — Signup** | Account creation | Name, email, phone, target degree level, target countries | Enough to personalize the homepage and dashboard immediately |
| **2 — Core profile** | Prompted on first dashboard visit | Academic background, test scores, study preferences | University matching, scholarship matching, requirement checklists |
| **3 — Getting serious** | Prompted when shortlisting or applying | Financial context, personal details (NID, DOB, guardian info) | Loan eligibility checks, Student File readiness |
| **4 — Documents** | Prompted per-document, contextually — e.g. "add your bank statement" appears when a bank page needs it, not before | Document wallet uploads | Application readiness, agency sharing, cross-page requirement matching |

The 78% completeness state in the mockup reflects a student who has done Stages 1–2 fully, made a start on Stage 3, and is mid-way through Stage 4 — a realistic, not aspirational, snapshot.

---

## 3. Brief user journey

1. **Sign up** with the minimum needed to personalize the homepage (Stage 1 fields).
2. **Land on the dashboard**, prompted to complete the core profile — this is what turns generic university/scholarship lists into matched ones.
3. **Explore and shortlist** — as a student browses country and university pages, the platform quietly notices gaps ("add your IELTS score to see your real match") rather than blocking access.
4. **Start applying** — this is the natural trigger for financial and document fields, since they're now clearly relevant, not abstract.
5. **Documents accumulate in the wallet once, reused everywhere** — the same passport or bank statement satisfies a university's requirement checklist, a bank's eligibility check, and an agency's file, without re-uploading.
6. **Ongoing maintenance** — expiring documents (IELTS, bank statements) resurface as dashboard nudges, keeping the profile accurate without a manual audit.

---

## 4. Profile elements & documents — consolidated reference

### Personal details
| Field | Required? | Powers |
|---|---|---|
| Full name (passport form) | Required | Identity, application forms |
| Date of birth | Required | Age checks (e.g. loan applicant age limits) |
| Gender | Optional | — |
| Nationality | Required | Visa-route eligibility |
| NID / birth certificate no. | Required | Identity verification, Student File |
| Phone, email | Required | Contact, account recovery |
| Current city | Optional | Localized content |
| Parent/guardian name & phone | Optional | Parent View, financial co-applicant |

### Academic background
| Field | Required? | Powers |
|---|---|---|
| Current education level | Required | Matching engine (degree-level filter) |
| Institution, field of study | Required | Matching engine |
| CGPA + scale | Required | Eligibility checks (universities & scholarships) |
| Graduation year | Required | Intake-timeline planning |

### Test scores
| Field | Required? | Powers |
|---|---|---|
| IELTS overall + bands + test date | Required (or TOEFL/Duolingo alt.) | Eligibility checks; **expiry auto-tracked from test date** |
| GRE/GMAT | Optional | Program-specific eligibility |

### Study preferences
| Field | Required? | Powers |
|---|---|---|
| Target degree level | Required | Matching engine |
| Target countries | Required | Country page personalization, matching |
| Target field/major | Required | Matching engine |
| Target intake | Required | Backward-planned journey steps |
| Budget per year | Required | University cost filtering, loan eligibility |

### Financial context
| Field | Required? | Powers |
|---|---|---|
| Funding source | Required | Loan eligibility routing |
| Collateral available | Required for loan tools | Bank eligibility checker (exact same field used on the Financial Partners Hub) |
| Guardian's income bracket | Required for loan tools | Bank eligibility checker |
| Existing bank relationship | Optional | Pre-fills Student File flow |

### Agency connection
| Field | Required? | Powers |
|---|---|---|
| Connected agency (if any) | Optional | Agency-synced steps, document sharing |

### Documents
| Document | Required? | Powers |
|---|---|---|
| Passport | Optional but recommended | Identity, visa filing |
| IELTS/English certificate | Required | University & visa eligibility |
| Offer letter | Optional (appears once issued) | Bank Student File, visa filing |
| Bank statement, 6 months | Required for loans/visa | Bank eligibility, visa financial evidence |
| NID — applicant & guarantor | Required for loans | Bank product requirements |
| Academic transcripts | Required | University application |
| Statement of Purpose | Optional | University application |
| Recommendation letters | Optional | University application |

---

## 5. Privacy note

Every document defaults to **private**. Sharing with a connected agency is an explicit, per-document toggle the student controls — visible directly on each document card, not buried in settings. This is a direct extension of the trust commitments already built into the agency and bank pages, and should be treated as non-negotiable rather than a nice-to-have.

---

## 6. Open questions for the team

1. **Verification depth:** Do any documents (passport, transcripts) need manual review before being marked "verified," similar to how agency case files are reviewed — or is upload-and-trust sufficient at launch?
2. **Guardian access:** Should a parent/guardian be able to fill in the financial section directly via Parent View, rather than relaying numbers through the student?
3. **Re-verification cadence:** Bank statements and IELTS certificates expire — should there be an automated re-upload reminder cycle, and if so, how far in advance?

---

*Prepared as a companion to the working profile mockup (`student-profile.html`). The mockup reflects Samira Rahman's profile at 78% completion for continuity with the rest of the platform's reference persona.*
