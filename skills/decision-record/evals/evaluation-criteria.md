# Evaluation criteria

Use these criteria to assess whether the record is accurate and decision-useful.

## It must

- Distinguish a made decision from an open discussion.
- State the decision in a short, outcome-based form.
- Capture rationale only where supported by the source material.
- Record meaningful alternatives and their actual trade-offs.
- Preserve material risks, conditions, dissent, and uncertainty.
- Identify missing owners, dates, or decisions rather than guessing.
- Include practical next actions.
- Be concise enough that a future teammate can understand the decision quickly.

## It must not

- Invent consensus, evidence, owners, deadlines, or approval.
- Present a proposal as settled.
- Recast rejected options as obviously inferior when the source does not support that.
- Write generic risks that apply to any project.
- Turn the record into a full PRD, project plan, or meeting summary.
- Hide unresolved questions merely to make the decision look complete.

## Expected behaviour by example

### 01: Auth-provider decision

The output should record WorkOS as the chosen direction and preserve:

- The enterprise SSO and custom-SAML maintenance context
- The cost trade-off
- The decision to migrate in phases
- The unresolved migration-effort question
- A migration plan as the immediate next action

It should not invent precise costs, migration dates, or claims that WorkOS is objectively superior in all contexts.

### 02: Launch-scope decision

The output should record the focused release as the decision.

It should make clear that:

- The selected scope is based on validated user needs
- Notifications and AI summaries are deferred, not rejected forever
- The reduced scope is a deliberate trade-off against completeness
- Engineering and design still need to confirm delivery safety

It should not describe this as “launching an MVP” unless that term appears in the source material.

### 03: Unresolved decision

The output must set the status to **No decision yet**.

It should record:

- The decision that remains open
- The competing considerations
- The missing evidence
- The next fact-finding action

It must not select a plan tier or infer that broader access is preferred.