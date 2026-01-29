# Bug Reports — HyGo College QA Project

This folder contains defect reports identified during functional, validation, API, and network resilience testing of the HyGo College Role Based Management System.

The goal of this section is to demonstrate my ability to:
- Identify real production-level defects  
- Classify bugs correctly using Severity and Priority  
- Write clear, reproducible, developer-friendly bug reports  
- Link UI behaviour with backend/API behaviour

## Bug Report Structure

Each bug report in this folder follows a consistent structure:

- **Summary** — Clear description of the problem  
- **Environment** — Browser, OS, module, role, and tools used  
- **Preconditions** — Required system state before reproduction  
- **Steps to Reproduce** — Numbered, repeatable steps  
- **Expected Result** — Correct system behaviour  
- **Actual Result** — Observed incorrect behaviour  
- **Impact** — Business and user impact of the defect  
- **Severity & Priority** — Risk-based classification  
- **Evidence** — Screenshots or video references  

This format mirrors standard Jira bug reporting practices used in industry.

## Defect Categories Covered

The bugs in this folder include examples of:

- **Functional Defects**
  - Core workflow failures (Attendance, Results, User actions)

- **Validation Defects**
  - Invalid input handling (e.g., score values outside allowed range)

- **API Defects**
  - Backend validation failures identified through Postman testing

- **Network & Resilience Defects**
  - Offline and poor-network behaviour using Chrome DevTools throttling

This demonstrates both **UI + API correlation** and **non-functional testing skills**.

## Sample Bugs Included

| Bug ID | Module | Category | Description |
|------|------|---------|------------|
| BUG_NET_01 | Attendance | Network / UX | Infinite loading spinner when saving attendance in offline condition |
| BUG_RESULT_01 | Result | Validation / API | System allows submission of invalid score values greater than 100% |

## Tools Used

- Manual Functional Testing  
- Chrome DevTools (Network Throttling & Offline Simulation)  
- Postman (API Testing & Validation)  
- Jira-style defect documentation  

## Notes on Confidentiality

This project is an academic system built and tested as part of my postgraduate project and for knowledge/portfolio demonstration.  

## Author

**Joy Oghogho Omorogiuwa**  
QA Engineer | API & Functional Testing | ISTQB Foundation Certified  

