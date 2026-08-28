# Project Brief Contract

`PROJECT-BRIEF.md` is the living source of truth for discovery decisions. Keep it concise enough to review, precise enough to plan from, and current when decisions change.

## Required sections

Include sections when relevant:

1. Status and approval
2. Executive definition
3. Problem and evidence
4. Users and stakeholders
5. Value and success measures
6. Product surfaces and platforms
7. Primary journey
8. MVP scope
9. Explicit exclusions and future phases
10. Business rules
11. Experience, content, and brand direction
12. Technical, data, integration, and AI decisions
13. Security, privacy, accessibility, and compliance
14. Operations and release
15. Acceptance criteria
16. Risks, assumptions, dependencies, and open questions
17. Decision log

Omit irrelevant empty sections. Do not fill gaps with invented information.

## Decision log

Use a compact table:

| Date | Decision | Status | Rationale | Affected areas | Source |
|---|---|---|---|---|---|

Source can be `User`, `Existing project`, `Documentation`, or `Agent recommendation`.

## Approval

The brief is not approved merely because it exists. Record:

- `Draft` while discovery continues.
- `Awaiting approval` when the summary is ready.
- `Approved` only after explicit user confirmation.
- `Reopened` when a material approved decision changes.

Approval authorizes planning, not unrelated external or destructive actions.

## Handoff

After approval, generate a plan whose milestones trace directly to the MVP scope and acceptance criteria. If implementation uncovers a material product decision, pause that branch, reopen the relevant brief decision, and ask the user rather than silently changing scope.
