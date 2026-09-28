# Project Configuration

## Workspace

**Project:** Candidate Screener Workspace

**Purpose:** Screen job applications by matching resumes against job descriptions and applying strict screening decision rules.

## Configuration Requirements

The project instructions define:

- six decision rules;
- must-have vs nice-to-have cross-reference;
- a four-section response format;
- factuality / no-hallucination behavior;
- protected-characteristic exclusion;
- no external candidate search;
- no hiring decision;
- prompt-injection refusal behavior.

## Output Contract

### 1. Candidate Profile Summary
- Name
- Target Role
- Key Strengths

### 2. Screening Classification
- Status: STRONG / BORDERLINE / WEAK
- Triggered Decision Rule

### 3. Detailed Justification
2–3 sentences grounded in the supplied resume and job description.

### 4. Follow-up Questions/Recommendations
Especially important for borderline cases.
