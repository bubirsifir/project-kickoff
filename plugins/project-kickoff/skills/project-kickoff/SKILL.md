---
name: project-kickoff
description: Run adaptive project discovery before implementation for a new product, website, app, AI system, automation, API, ecommerce project, or material change to an existing project. Use when the user wants to start, define, scope, plan, or clarify a project before building. Do not use for a narrowly specified implementation or bug fix whose requirements and acceptance criteria are already clear.
metadata:
  short-description: Adaptive discovery before implementation
---

# Project Kickoff

Turn an idea or change request into an approved, decision-backed project brief before implementation. Match the user's language and technical level.

## Choose the operating mode

Inspect the request and any project files first when available. Then choose one mode:

- **Idea discovery:** the user has an early or unclear idea.
- **New project definition:** the outcome is understood but scope and decisions are incomplete.
- **Existing project change:** inspect the current system and clarify the desired change, constraints, compatibility, and acceptance criteria.
- **Ready-to-build check:** requirements appear complete; verify only decisions that could materially change the solution.

Do not force a full interview for a small, already-clear task. Never ask for information already provided or reliably discoverable from the workspace.

## Run adaptive discovery

1. Summarize the project in one or two sentences and state the mode you inferred.
2. Identify unresolved decisions that materially affect product direction, scope, platform, architecture, risk, cost, or acceptance.
3. Ask one main decision question at a time.
4. When useful, offer 2–4 mutually exclusive choices, explain their consequences briefly, and recommend one based on current evidence.
5. Let the user answer freely; choices are aids, not constraints.
6. Adapt the next question to the answer. Skip irrelevant branches.
7. Record decisions continuously in `PROJECT-BRIEF.md` when file writes are authorized. Otherwise maintain a structured draft in the conversation.
8. Stop interviewing when the remaining unknowns can safely be treated as implementation choices.
9. Present a decision summary, open risks, proposed delivery phases, and explicit approval gate.
10. Do not begin implementation until the user approves the brief, unless the user explicitly instructs you to proceed without that gate.

Read [interview-method.md](references/interview-method.md) for question discipline, decision ownership, and stopping rules.

## Route by project type

Infer one or more project types from the user's explanation. If unclear, begin with: “What kind of project do you want to create? You can describe the idea in a few sentences; it does not need to be fully formed.”

Use [project-routes.md](references/project-routes.md) to select relevant domains for websites, SaaS/web apps, mobile apps, ecommerce, AI products, automations, APIs, content products, and existing systems. Do not read every route as a mandatory checklist.

## Resolve platform and surface decisions early

After purpose and users are understood, determine where and how the product will be used. Distinguish responsive web, PWA, native or cross-platform mobile apps, desktop apps, APIs, browser extensions, kiosks, and other device surfaces. Also distinguish public website, customer app, staff app, admin panel, partner portal, and developer API.

Read [platform-routing.md](references/platform-routing.md) when the project has a user interface, multiple user groups, mobile requirements, or unclear “web + mobile” language.

Do not ask the user to choose a framework before establishing the product need. Recommend technology after usage, device capabilities, distribution, team constraints, budget, and delivery sequence are known.

## Cover the right decision levels

Select only the domains that can change the outcome:

- purpose, problem, users, and context;
- value proposition, alternatives, business model, and success metrics;
- scope, priority, workflows, roles, permissions, and content;
- brand, design direction, accessibility, and interaction expectations;
- platform, architecture, data, integrations, AI behavior, security, privacy, and compliance;
- operations, support, analytics, rollout, ownership, budget, schedule, and future phases.

Read [decision-domains.md](references/decision-domains.md) to identify high-impact questions and project-specific omissions. Treat it as a decision map, not a questionnaire.

## Separate decision ownership

Classify unresolved items before asking:

- **User decision:** business goal, target audience, scope, risk tolerance, brand, pricing, launch priority, or another intent-dependent choice.
- **Joint decision:** platform strategy, experience direction, architecture tradeoff, rollout sequence, or another choice where recommendation and user approval both matter.
- **Implementation decision:** naming, folder organization, routine library choice, or another reversible detail the agent can decide safely.

Ask the user about user and high-impact joint decisions. Make ordinary implementation decisions yourself, record important ones as agent-selected, and avoid burdening the user with low-level questions.

## Maintain the brief

Use [brief-contract.md](references/brief-contract.md) for the living `PROJECT-BRIEF.md` structure. Copy [PROJECT-BRIEF.template.md](assets/PROJECT-BRIEF.template.md) when a project needs a fresh file.

Record each material decision with its rationale, status, affected areas, and source. Use these statuses:

- `Confirmed` — explicitly decided by the user.
- `Recommended` — proposed but awaiting approval.
- `Assumed` — temporarily adopted; must be visible and low-risk.
- `Open` — unresolved and material.
- `Deferred` — intentionally postponed to a later phase.

If a new answer conflicts with an earlier decision, surface the conflict and update the brief after resolution. Do not keep mutually inconsistent requirements silently.

## Approval gate

Before implementation, present:

1. concise product definition;
2. target users and core problem;
3. selected platforms and product surfaces;
4. primary user journey;
5. MVP scope and explicit exclusions;
6. key business, experience, technical, data, and security decisions;
7. success and acceptance criteria;
8. risks, assumptions, dependencies, and open decisions;
9. proposed phases and recommended first milestone.

Ask for approval or corrections. After approval, mark the brief approved with the date and convert it into an actionable implementation plan. Preserve authorization boundaries: approval of the brief does not itself authorize deployment, external messages, purchases, or destructive changes.

## Quality bar

A successful kickoff is concise but decision-complete. It should prevent expensive rework without turning into an endless interview. Prefer evidence and recommendations over generic questions. Challenge contradictory scope or unnecessary platform expansion respectfully. Do not invent market facts, legal requirements, integrations, budgets, deadlines, or stakeholder approval.

Treat familiar AI-generated product patterns as unconfirmed assumptions, not defaults. Do not introduce a dashboard, card grid, oversized hero, pill-heavy interface, gradient-led visual language, generic marketing claims, or fashionable technology merely because it is common in generated projects. Derive information architecture, interaction patterns, visual direction, content, and technical choices from the confirmed users, problem, context, and constraints. These patterns are not forbidden when the brief gives them a real purpose; require a reason instead of applying them automatically.
