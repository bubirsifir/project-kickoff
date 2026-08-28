# Adaptive Interview Method

## Objective

Reach the smallest set of confirmed decisions that makes the next delivery phase safe and coherent. The interview is a branching conversation, not a fixed intake form.

## Start

Use known context first. Inspect existing files when relevant and authorized. Open with a compact reflection:

> I understand this as [project/change] for [users] to [outcome]. I will first resolve the decisions that affect scope and architecture, then show you the brief for approval.

If even the project category is unclear, ask what the user wants to make. If the category is clear, do not ask them to label it again.

## Question design

Ask one main decision per turn. A question may contain tightly related subparts only when separating them would be artificial, such as desired launch market and language.

Good questions:

- change a downstream decision;
- can be answered without specialized jargon;
- explain why the choice matters;
- include a recommendation when evidence supports one;
- allow a free-form answer.

Avoid:

- asking the user to fill a long template;
- presenting the entire backlog of questions at once;
- asking about information already supplied;
- asking low-level technical choices before product needs;
- treating every possible feature as required;
- repeating a question because the answer was phrased indirectly;
- continuing after decisions are sufficient to proceed.

## Recommended choice format

Use options when they reduce cognitive load:

> Where should the first version be available?
>
> A. Responsive web — fastest validation and one deployable surface.  
> B. Web + native mobile — broader distribution, higher initial cost.  
> C. Mobile first — suitable when device capabilities are central.  
>
> Based on [known reason], I recommend A for the first release.

Do not recommend an option merely to appear decisive. State uncertainty when evidence is insufficient.

## Priority

Ask in this order unless project context demands otherwise:

1. Decisions that can invalidate the entire direction.
2. Scope and user-flow decisions.
3. Platform, data, security, integration, cost, or schedule decisions.
4. Brand, content, and presentation decisions.
5. Reversible implementation details, usually decided by the agent.

## Depth control

Adjust the interview to the user:

- Translate technical choices into consequences for nontechnical users.
- Offer architecture detail to technical users when it affects their decision.
- If the user says “you decide,” choose the most defensible option and record the rationale.
- If the user wants speed, ask only blocking questions and label low-risk assumptions.
- If the domain is regulated or high-risk, do not reduce essential privacy, security, compliance, or human-oversight questions.

## Conflict handling

When answers conflict:

1. Name the two conflicting decisions plainly.
2. Explain the practical consequence.
3. Recommend a resolution or phased alternative.
4. Ask the user to confirm the resolution.
5. Update the decision log; do not preserve both as active requirements.

## Stop conditions

Stop asking questions when:

- the first milestone has a clear user, outcome, platform, scope, and acceptance criteria;
- material data, security, integration, and operational risks are resolved or explicitly deferred;
- remaining decisions are reversible implementation choices;
- additional questions would not alter the next delivery phase.

Do not stop merely because a target number of questions has been reached. Do not continue merely because the decision catalog contains unused topics.
