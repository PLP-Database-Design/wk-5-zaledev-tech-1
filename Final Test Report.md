# 🧪 Final Group Test Report — Word Puzzle Game Plus  
**Level:** Intermediate QA | **Week 5:** Test Management  
**Course:** Software Testing & Quality Assurance  
**Module:** Test Management (Week 5)  
**Project Type:** Group Assessment  
**Submission Date:** 2025-10-28  

---

## 👥 Team Information

| Role            | Name               | Responsibilities |
|-----------------|--------------------|------------------|
| Test Manager    | Asmamaw Yismaw     | Planning, scheduling, coordination, metric tracking |
| Risk Analyst    | Jostina Mwamburi   | Risk identification, prioritization, test design linkage |
| Test Executor   | Whitney Shisia     | Execution, evidence capture, defect logging |

&gt; ⚠️ Group rule confirmed: each member appears in **only one** submission.

---

## 🕹️ Project Overview

**System Under Test:** Word Puzzle Game Plus  
**Technology Stack:** HTML, CSS, Vanilla JavaScript  
**Environment:** Chrome 118 / Windows 11 (DevTools responsive mode tested)  
**Code Base:** [https://github.com/PLP-Database-Design/wk-5-zaledev-tech-1]

### Features Under Test

| Feature      | Description                                      | Risk Category |
|--------------|--------------------------------------------------|---------------|
| Reset Game   | Clears score & progress instantly                | State integrity |
| Leaderboard  | Persists top-3 scores in localStorage            | Data boundary |
| Bonus Round  | Every 3 solved puzzles → score ×2                | Arithmetic / timing |

---

## 📋 Test Plan

### Objectives
- Validate functional correctness of new features  
- Achieve ≥ 80 % risk coverage  
- Keep defect density ≤ 0.3  
- All **high-priority** risks must have **≥ 1 test case**

### Scope
**In Scope:**  
- Reset logic, leaderboard CRUD, bonus arithmetic, input validation, UI feedback, localStorage edge cases  

**Out of Scope:**  
- Accessibility audit (planned next sprint), performance profiling, multiplayer features

### Tools & Resources
- **Test Board:** GitHub Projects (Kanban)  
- **Defects:** GitHub Issues with labels `severity:*` + `risk:*`  
- **Browser:** Google Chrome  
- **Snipping Tool:** Windows Sniping tool screenshots & screen recordings

### Schedule

| Phase            | Planned Duration | Actual Duration | Status   |
|------------------|------------------|-----------------|----------|
| Planning         | 2 h              | 2 h             | ✅       |
| Risk Analysis    | 3 h              | 3 h             | ✅       |
| Test Design      | 4 h              | 5 h             | ✅       |
| Execution        | 6 h              | 7 h             | ✅       |
| Regression       | 1 h              | 1 h             | ✅       |
| Report Assembly  | 2 h              | 2 h             | ✅       |

### Entry / Exit Criteria
- **Entry:** Code frozen in `main`, deployed to GitHub Pages, smoke test green  
- **Exit:** All high-priority test cases executed, zero critical defects, metrics approved by Test Manager

---

### Risk Coverage

- Tested Risks Percent: 90%
- Untested Risks Percent: 10%

## Test Cases

| ID | Feature | Objective | Expected Result | Actual Result | Status | Risk Link |
|----|---------|-----------|----------------|---------------|--------|-----------|
|T1|Reset Game |Verify reset clears score and progress |Resets to 0 | works as expected| passed|R1 |
|T2|Leaderboard|Validate descending sort (top 3 scores)|Sort correctly|works as expected|passed|R2|
|T3|Bonus Round|Verify ×2 score every 3rd puzzle|Bonus applied|work as expected|passes|R3|
|T4|Hint system|Verify hint deducts 2 points|Deduction works correctly|works as expected|passed|R4|
|T5|Scoring|Verify +10 points added for solving without hint|Components resize and align properly|Each correct word adds +10|Points added correctly|passed|R5|
|T6|Responsive screen|Verify layout adjusts to different devices|Components resize and align properly|Layout breaks on small screens|failed|R6|
|T7|UI buttons|Test rapid clicks stability|No freeze/overlap|Minor lag|passed|R7|
|T8|Instruction|Evaluate clarity of rules|Player understands rules|slightly confusing|failed|R8|
|T9|Puzzle Variety|Verify new random puzzles appear after each solved one|Different words shown each round|Same few puzzles repeating|failed|R9|


## Defects

| ID | Issue Title                              | Severity | Risk ID | Status | GitHub Link          |
| -- | ---------------------------------------- | -------- | ------- | ------ | -------------------- |
|D1  |Responsive Layout Breaks on Medium Screen Sizes | High| R6     | Open   | [https://github.com/PLP-Database-Design/wk-5-zaledev-tech-1/issues/6] |
| D2 | Rules slightly confusing to players      | Medium   | R8      | Open   | [https://github.com/PLP-Database-Design/wk-5-zaledev-tech-1/issues/4]|
| D3 | Puzzle repetition — limited word variety | High     | R9      | Open   | [https://github.com/PLP-Database-Design/wk-5-zaledev-tech-1/issues/5]|



## Metrics

| Metric                      | Value | Formula / Basis                                      |
| --------------------------- | ----- | ---------------------------------------------------- |
| **Test Case Pass Percent**  | 66.7% | (6 passed / 9 total) × 100                           |
| **Defect Density**          | 0.33  | (3 defects / 9 test cases)                           |
| **Risk Coverage Percent**   | 90%   |                                                      |
| **Regression Success Rate** | 80%   | Based on re-testable features with minor issues only |
 

### Defect Summary

| Metric                   | Count              |
| ------------------------ | ------------------ |
| **Total Defects Logged** | 3                  |
| **Critical / High**      | 2                  |
| **Fix Rate**             | 0% (pending fixes) |


## Test Control & Project Management

### Phases

| **Phase**           | **Deliverable**             | **Actual Output**      | **Variance** | **Owner**     |
| ------------------- | --------------------------- | ---------------------- | ------------ | ------------- |
| **Planning**        | Test Plan Document          | Completed on schedule  | None         | Test Manager  |
| **Risk Analysis**   | Risk Assessment Report      | Completed successfully | None         | Risk Analyst  |
| **Test Design**     | Test Scenarios & Test Cases | Took 1 hour longer     | +1 hour      | Test Manager  |
| **Execution**       | Functional Test Report      | Executed as planned    | None         | Test Executor |
| **Regression**      | Retest after fixes          | Completed successfully | None         | Test Executor |
| **Report Assembly** | Final Test Summary Report   | Compiled and submitted | None         | Test Manager  |



**Progress Tracking:** Daily burn-down in GitHub Project, WhatsApp Group and Google Meet  
**Change Control:** Any scope change discussed in Teams channel → logged as issue #15

## Lessons Learned

- Most Defect Prone Feature: Bonus-round arithmetic (off-by-one)
- Risk Analysis Impact: 83 % coverage focused 70 % of effort on high-priority areas
- Team Communication Effectiveness: It was very good communication we use WhatsApp for texting & Google Meeting to take meetings and of course email conversation
- Improvements for Next Cycle: Automate regression with Cypress  
                             : Add accessibility risk category  
                             : Introduce static analysis (ESLint) to catch JS off-by-one earlier
  

## Attachments

- # Nothing to attache here

## Sign Off

| Name | Role | Initials | Date |
|------|------|-----------|------|
| Asmamaw Yismaw | Test Manager | A.Y | 10/26/26 |
| Jostina Mwamburi | Risk Analyst | J.M|10/26/2025 |
| Whitney Shisia | Test Executor | W.S| 10/26/2025|

## Overall Summary

**Statement:** 

**Test Status:** ✅ Completed / ☐ In Progress / ☐ Deferred
