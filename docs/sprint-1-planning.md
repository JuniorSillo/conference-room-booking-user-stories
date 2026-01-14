# Sprint 1 Planning Session

**Date:** 14 January 2026
**Sprint Goal:**  Enable Employees to book and manage conference rooms efficiently (recurring bookings, cancellations, and equipment requirements) while also allowing Administrators to monitor and resolve conflicts.

## Attendees
- Product Owner: Junior Sillo
- Scrum Master: Junior Sillo
- Development Team: Junior Sillo (Full-stack developer)

## Velocity Target
Intended velocity: **18-22 story points**

## Selected User Stories

| Story # | Title                                | Story Points |
|---------|--------------------------------------|--------------|
|1        | Story #1 Room Booking System         | 3            |
|2        | Story #2 Recurring Bookings Setup    | 5            |
|4        | Story #4 Booking Cancellation        | 2            |
|5        | Story #5 Room Equipment Requirements | 3            |
|6        | Story #6 Admin Dashboard Viewing     | 5            |
|9        | Story #9 Booking Conflicts Resolution| 2            |
| Total   |                  -                   | **20**       |

## Dependencies
- Story #2, #4, #5 depends on completion of #1
- Story #9 depends on #1 and #6

## Risks

| Risk                                         | Probability | Impact  | Mitigation                                       |
|----------------------------------------------|-------------|---------|--------------------------------------------------|
| Underestimation of recurring logic (Story #2)| Medium      | High    | Break into smaller subtasks, early testing       | 
| Time zone bugs in booking (Story #1)         | Medium      | High    | Use moment time-zone library, adding tests early |
| Scope creep on dashboard visuals (Story #6)  | Low         | Medium  | Strict acceptance criteria, defer fancy charts   |
| Solo Developer burnour                       | Medium      | High    | Strict daily standups, time-box work, take breaks|

## Standup Cadence
- Time: 9:00 AM - 9:15 AM (Weekly)
- Format: Scrum Standup
    - What did I do Yesterday?
    - What will I do Today?
    - Any blockers?