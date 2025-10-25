# 🧪 Final Group Test Report Template — Word Puzzle Game Plus

**Level:** Intermediate QA | **Week 5:** Test Management

**Course:** Software Testing & Quality Assurance  
**Module:** Test Management (Week 5)  
**Project Type:** Group Assessment  
**Submission Date:** 2025-10-28

## Team Information

| Role | Name | Responsibilities |
|------|------|------------------|
| Test Manager | | Planning, scheduling, coordination, metric tracking |
| Risk Analyst | | Risk identification, prioritization, test design linkage |
| Test Executor | | Execution, evidence capture, defect logging |

## Group Rules

- Each student must belong to only one group.
- Duplicate membership or multiple submissions will result in invalidation.
- Every group member must contribute towards this project

## Project Overview

**System Under Test:** Word Puzzle Game Plus  
**Technology Stack:** HTML, CSS, JavaScript  
**Environment:** Chrome Browser (Desktop)

### Features Under Test

| Feature | Description | Risk Category |
|---------|-------------|---------------|
| Reset Game | Clears score and progress instantly | |
| Leaderboard | Stores top 3 scores in localStorage | |
| Bonus Round | Every 3 puzzles → doubles score | |

## Test Plan

### Objectives

- 

### Scope

**In Scope:**
- 

**Out of Scope:**
- 

### Tools & Resources

- 

### Schedule

| Phase | Planned Duration | Actual Duration | Status |
|-------|------------------|-----------------|--------|
| | | | |

## Risk Analysis

### Risks

| ID | Feature | Risk Description | Likelihood | Impact | Priority | Mitigation Strategy |
|----|---------|------------------|------------|--------|----------|---------------------|
| R1|Reset Game |Reset button fails to clear score or puzzle progress correctly |high|high |high |Conduct repeated reset tests; verify counters reset to zero and game state reinitialized |
|R2|Leaderboard|Scores not stored or sorted correctly in localStorage|high|high|high|Test multiple scores|
|R3|Bonus Round|Bonus not triggered after every 3 puzzles|medium|medium|medium|Test sequences (3rd, 6th, 9th puzzles); confirm doubled score applied|
|R4|Hint system|Hint deduction (-2 points) misapplied or double-counted|medium|medium|medium|Verify hint deduction sequence and total score after use|
|R5|Scoring|Score overflow or negative value after repeated bonuses|low|low|low|Add boundary checks and validation for score value|
|R6|Responsive screen|Game layout not adapting correctly to various screen sizes|high|high|high|Apply responsive CSS grid/flexbox; test on multiple devices and breakpoints; use Chrome DevTools to simulate screens|
|R7|UI Buttons|Buttons freeze or overlap after rapid clicks|medium|medium|medium|Conduct rapid-click stress test; debounce actions|
|R8|Instructions / Rules|Player misinterprets hint cost or bonus rule|medum|medium|medium|Improve wording in Rules section; add in-game tooltip|


### Risk Coverage

- Tested Risks Percent: 
- Untested Risks Percent: 

## Test Cases

| ID | Feature | Objective | Expected Result | Actual Result | Status | Risk Link |
|----|---------|-----------|----------------|---------------|--------|-----------|
| | | | | | | |

## Defects

| ID | Issue Title | Severity | Risk ID | Status | GitHub Link |
|----|-------------|----------|---------|--------|-------------|
| | | | | | |

## Metrics

- Test Case Pass Percent: 
- Defect Density: 
- Risk Coverage Percent: 
- Regression Success Rate: 

### Defect Summary

- Total Defects Logged: 
- Critical High: 
- Fix Rate: 

## Test Control & Project Management

### Phases

| Phase | Deliverable | Actual Output | Variance | Owner |
|-------|-------------|---------------|----------|-------|
| | | | | |

**Progress Tracking Method:**  
**Change Control Notes:**

## Lessons Learned

- Most Defect Prone Feature: 
- Risk Analysis Impact: 
- Team Communication Effectiveness: 
- Improvements for Next Cycle: 

## Attachments

- 

## Sign Off

| Name | Role | Initials | Date |
|------|------|-----------|------|
| | Test Manager | | |
| | Risk Analyst | | |
| | Test Executor | | |

## Overall Summary

**Statement:** 

**Test Status:** ☐ Completed / ☐ In Progress / ☐ Deferred
