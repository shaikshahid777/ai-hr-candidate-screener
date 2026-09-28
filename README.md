# AI HR Candidate Screener

An assessment-ready AI HR Candidate Screener built in a ChatGPT Project workspace. It matches uploaded resumes against job descriptions, applies six deterministic screening rules, and returns a structured, factual, bias-aware screening summary.

## Project Links

- 🎥 [Loom Demo](https://www.loom.com/share/12321feeaa3540c29236be66419707da)
- 🤖 [ChatGPT Project](https://chatgpt.com/share/6aba60f3-4c60-83ee-9a8b-47840f597c9a)

## Core Workflow

```text
Job Description + Candidate Resume(s)
                ↓
        Requirement Matching
                ↓
      Six Decision Rules
                ↓
     STRONG / BORDERLINE / WEAK
                ↓
   Structured Screening Output
```

## Decision Rules

| Rule | Scenario | Classification / Action |
|---|---|---|
| Rule 1 | Missing email or phone | BORDERLINE; request missing contact details |
| Rule 2 | 2+ year experience shortfall + no relevant certification | WEAK; archive according to rule |
| Rule 3 | No work experience + 3+ relevant certifications | BORDERLINE; recommend 15-minute technical screening call |
| Rule 4 | Matches multiple open positions | Use strongest skill match; list alternative fits |
| Rule 5 | Vague tasks / weak evidence | BORDERLINE; generate 2–3 behavioral questions |
| Rule 6 | All must-haves + 80%+ nice-to-haves | STRONG; apply configured fast-track action |

## Required Output

Every screening follows four sections:

1. **Candidate Profile Summary**
2. **Screening Classification**
3. **Detailed Justification**
4. **Follow-up Questions/Recommendations**

## Validation Coverage

- ✅ Strong Match — Rule 6
- ✅ Weak Data — Rule 2
- ✅ Certifications vs Experience — Rule 3
- ✅ Multiple Options — Rule 4
- ✅ Unclear Tasks — Rule 5
- ✅ Missing Contact Information — Rule 1

## Guardrails

The project configuration requires grounded evaluation from uploaded sources, no invented qualifications, and no use of age, gender, location, or other protected characteristics in screening. The screener is also configured not to perform external candidate searches or make hiring decisions.

## Repository Structure

```text
.
├── README.md
├── docs/
│   ├── assessment-notes.md
│   ├── project-configuration.md
│   ├── source-materials.md
│   └── validation-report.md
├── 01_*  Job description
├── 02_*  Strong candidate resume
├── 03_*  Validation resume
├── 04_*  Borderline candidate resume
├── 05_*  Missing-contact scenario
├── 06_*  Rule 2 scenario
├── 07_*  Open position — AI Automation Analyst
├── 08_*  Open position — API Integration Specialist
├── 09_*  Multiple-options candidate
└── AI_HR_Candidate_Screener_LMS_Submission(1).pdf
```

## Assessment Deliverables

The repository contains the project source materials and LMS submission evidence. The Loom and ChatGPT Project links provide the live demonstration and configured workspace context.

---
Built as an AI HR screening capstone focused on structured requirements matching, deterministic decision rules, factuality, and bias-aware evaluation.
