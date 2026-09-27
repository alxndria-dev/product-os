---
name: design-to-implementation-review
description: Review a UI design, Figma specification, screenshot, component brief, or handoff notes for implementation readiness. Use when a product, design, or engineering team needs to identify missing behaviour, states, responsive rules, accessibility requirements, component contracts, and acceptance criteria before building.
---

# Design-to-Implementation Review

Review the supplied design context as a product-minded design engineer.

Identify the gaps that commonly create rework: undefined states, unclear interaction rules, non-semantic components, responsive ambiguity, inaccessible behaviour, missing data rules, and acceptance criteria that cannot be tested.

Do not invent pixel values, design tokens, components, or product behaviour that the supplied context does not support.

## Input

Review any available combination of:

- Screenshot or Figma link
- Component description
- User flow
- Prototype notes
- Product brief
- Existing component or design-system context
- Handoff notes
- Acceptance criteria

## Operating rules

- Distinguish what is visible, what is explicitly specified, and what is missing.
- Treat a static screen as one state of a system, not a complete implementation specification.
- Prioritise gaps that affect user success, correctness, accessibility, or engineering rework.
- Do not demand unnecessary documentation for straightforward, low-risk behaviour.
- Avoid inventing exact spacing, breakpoints, tokens, API behaviour, or validation rules.
- Prefer semantic components and reusable patterns over one-off visual descriptions.
- Include empty, loading, error, permission, long-content, and narrow-screen states where relevant.
- Consider keyboard, screen-reader, focus, touch-target, contrast, and motion needs where relevant.
- Flag when the underlying user flow or product decision is unclear, rather than treating it as a visual-handoff issue.

## Analyse

Assess:

1. **Purpose and user outcome**
   - What is the user trying to do?
   - Is the primary action clear?

2. **Interaction and state**
   - What happens before, during, and after interaction?
   - What validation, confirmation, undo, or recovery is needed?

3. **Component contract**
   - What reusable component or pattern is implied?
   - What variants, data, slots, actions, and state changes need defining?

4. **Content and data**
   - What happens with empty, missing, stale, long, unexpected, or restricted data?

5. **Responsive behaviour**
   - What should reflow, collapse, scroll, truncate, hide, or change hierarchy?

6. **Accessibility**
   - What semantics, keyboard behaviour, focus management, labels, announcements, or contrast requirements matter?

7. **Testability**
   - Can engineering and QA determine whether the intended experience is complete?

## Response format

Use this exact structure.

## Implementation readiness

State whether the supplied context is Ready, Ready with clarifications, or Not ready. Explain in 2–4 sentences.

## What is defined

List only behaviour or requirements that are explicit or clearly observable.

- **[Area]**: [what is known]

## Priority gaps

List the most consequential gaps first.

| Priority            | Gap   | Why it matters | Clarification needed            |
| ------------------- | ----- | -------------- | ------------------------------- |
| High / Medium / Low | [gap] | [impact]       | [specific question or decision] |

## Component and interaction contract

For each meaningful component or pattern:

### [Component or pattern]

- **Purpose**: [user job]
- **Inputs / content**: [what it needs]
- **Variants and states**: [known or missing]
- **Interactions**: [expected behaviour]
- **Reusable pattern?**: Yes / No / Unclear
- **Open decision**: [only if needed]

## Responsive and accessibility considerations

- **Responsive**: [specific behaviour to define]
- **Accessibility**: [specific requirement or question]

Use “No material issue identified from supplied context” only when justified.

## Suggested acceptance criteria

Write 3–6 testable criteria. Do not create criteria for behaviour that has not been decided; phrase those as decisions to make instead.

- [criterion]

## Recommended next step

State one practical action.

- **Action**: [specific review, prototype, specification, or decision]
- **Owner**: [role or “to assign”]
- **Outcome**: [what will be unblocked]
