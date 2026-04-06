# CSC8632 – Data Science in the Wild | LaunchPad Nexus

This repository contains the group project submission for the **Data Science in the Wild** module (CSC8632). The project is **LaunchPad Nexus** — an AI-powered graduate employability web application built for the Newcastle University Careers & Employability Service.

**Student:** Vivan Kushal Heneger | **Student ID:** 250469037  
**Team:** Pranit Chatterjee · Vivan Kushal Heneger · Xiaokai Chen · Archie Barnett · Ajay Sivakumar · Rajbala Jadhav  
**Client:** Newcastle University Careers & Employability Service  
**Submission Date:** 20th March 2026

---

## Repository Structure

```
├── GroupWork_Final.pdf                        # Group Project Report
├── LaunchPad_Nexus_Executive_Report.pdf       # Executive Report
├── Reflective_Log_Vivan_Kushal_Heneger.pdf    # Individual Reflective Log
└── README.md
```

---

## Project Overview

**LaunchPad Nexus** is a student-built AI-supported web application that helps final-year and recent graduates targeting data and technology roles turn noisy job descriptions into clear, personalised **7-day action plans**.

### The Problem

Most existing careers support is generic, fragmented, and not available at the exact moment a student is reviewing a specific job description. Students targeting data and technology roles face:

- Overwhelming job descriptions with aspirational or duplicated requirements
- No personalised guidance on what to prioritise
- Lack of feedback and accountability in the job-search process
- A confidence gap, particularly for students from non-traditional backgrounds

### The Solution

LaunchPad Nexus addresses this by providing an on-demand, AI-powered tool that:

1. Collects a structured student profile (goals, skills, experience, timeline)
2. Accepts a real job description input
3. Uses an LLM (Google Gemini) to filter out noise and identify what genuinely matters
4. Generates a personalised **3–5 step weekly action plan**
5. Captures feedback to improve recommendations over time

---

## How It Works

```
Student Profile (3-Step Wizard)
    ↓
Job Description Input (paste or upload)
    ↓
Gemini LLM Analysis
    ├── JD De-Noising: filters aspirational/unrealistic requirements
    ├── Gap Diagnosis: compares filtered JD against student profile
    └── Red Flags Detection: title mismatches, vague requirements, missing salary
    ↓
Output: Personalised 7-Day Action Plan
    ├── Role & Company at a Glance
    ├── What You Must Focus On vs What to Ignore
    ├── Numbered action steps with estimated time & rationale
    └── Sub-steps with direct resource links (datasets, tutorials, docs)
    ↓
Feedback Loop: tracks completed actions → improves future recommendations
```

---

## Technology Stack

| Component | Technology |
|---|---|
| LLM / AI Layer | Google Gemini (via Google AI Studio) |
| Backend Database | Firebase |
| Frontend | Structured multi-step web form (Google AI Studio app builder) |
| Prototype URL | [LaunchPad Nexus App](https://ai.studio/apps/4d90c155-d85e-4e87-9d06-9dc16a439c8d) |
| Survey Tool | Google Forms |

---

## Key Features

- **JD Noise Filtering** — identifies 'unicorn hunt' job descriptions and separates must-have from aspirational requirements
- **Personalised Action Plans** — matched to the student's specific profile, skills, and experience level
- **Red Flags Panel** — highlights issues like title mismatches, vague requirements, or missing salary
- **Resource-Linked Steps** — each action step includes direct links to Kaggle datasets, tutorials, and documentation
- **Feedback Loop** — captures which actions students complete to improve future recommendations

---

## Research & Validation

### User Survey
A primary research survey was distributed via Google Forms to final-year and recent graduate students.

**Key findings (6 responses):**
- **50%** identified "knowing where to start" as their biggest job-search challenge
- **66.6%** said they would be likely or very likely to use a tool like this weekly
- **50%** identified lack of real-world experience (projects, internships, portfolio) as their most pressing gap

> Survey: [LaunchPad Nexus Job Search Support](https://forms.gle/tFB34CPSQ5Pxeg8r5)

### Design Frameworks Used
- Empathy Map Canvas
- Customer Journey Map (6 stages: Awareness → Outcome)
- Value Proposition Canvas
- Business Model Canvas

---

## MVP Implementation Plan

| Phase | Timeline | Key Activities |
|---|---|---|
| 1: Setup & Partnerships | Weeks 1–2 | Confirm university support, LLM API access, case-study database, intake form |
| 2: Build & Test | Weeks 3–5 | Backend recommendation engine, LLM integration, internal testing (5–10 students) |
| 3: Pilot Launch | Weeks 6–9 | Recruit 50+ pilot users, weekly tool use, collect feedback |
| 4: Evaluate & Refine | Weeks 10–12 | Analyse engagement data, action completion rates, produce evaluation report |

### Success Metrics

| Metric | Target |
|---|---|
| User engagement | 50+ students onboarded in pilot |
| Action completion | >60% complete at least 2 of 3 weekly actions |
| Perceived clarity | Increased confidence score post-use |
| Return usage | >40% return for a second weekly plan |

---

## Future Scope

- AI-generated role-specific skill assessments
- Gamified progress tracking (streaks and milestones)
- Recruiter follow-up assistant
- Peer learning features connecting students targeting similar roles
- White-label institutional dashboard (B2B) for other universities

---

## Individual Contribution (Vivan Kushal Heneger)

- Led report writing and structured all four sections of the group report
- Contributed to Empathy Map, Value Proposition Canvas, and Business Model Canvas
- Conducted early-stage user research by distributing the survey via LinkedIn
- Participated in all wrap-up sessions and contributed to the group presentation
- Reflected on working independently vs. group decision-making for future dissertation work

---

## References

- AGCAS (2023) Graduate labour market trends
- CBI (2022) Employer perspectives on graduate recruitment
- HESA (2024) Graduate outcomes: What do graduates do?
- ICO (2023) Guide to the UK GDPR
- ISE (2023) Student development survey
- Crawford & Fink (2019–2020) Employability Skills and Students Critical Growth Areas
- Shury et al. (2017) Planning for success: Graduates' career planning and its effect on graduate outcomes
- Smith, McKnight & Naylor (2000) Graduate Employability: Policy and Performance in Higher Education in the UK

---

## Compliance

All student data collected during the pilot is anonymised, participation is voluntary, and the tool complies fully with **UK GDPR** (ICO, 2023).
