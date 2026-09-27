# Evaluation criteria

Use these criteria to assess whether the review prevents meaningful implementation ambiguity.

## It must

- Distinguish visible design details from specified behaviour and missing requirements.
- Identify the user outcome and primary interaction.
- Prioritise gaps by impact on user success, correctness, accessibility, or delivery risk.
- Consider relevant loading, empty, error, permission, long-content, and responsive states.
- Identify semantic, keyboard, focus, and screen-reader requirements where appropriate.
- Suggest reusable component contracts when a pattern is evident.
- Write testable acceptance criteria.
- Stay proportionate to the complexity of the supplied design.

## It must not

- Invent exact dimensions, breakpoints, tokens, APIs, or business rules.
- Turn every static screen into an exhaustive specification exercise.
- Focus only on visual styling.
- Treat a Figma screen as sufficient evidence of interaction behaviour.
- Assume desktop patterns will work on narrow screens.
- State that an experience is accessible without assessing relevant behaviour.
- Write vague acceptance criteria such as “works correctly” or “is responsive.”

## Expected behaviour by example

### 01: Dashboard insight card

The output should identify:

- Loading, empty, error, and unavailable-evidence states
- Whether source count links to inspectable evidence
- Permissions and restricted-source behaviour
- How long text and many sources are handled
- Side-panel focus management, keyboard behaviour, and escape handling
- Narrow-screen behaviour for the two-column grid and side panel
- The distinction between an AI-generated claim and its supporting sources

It should not invent an exact card height or mobile breakpoint.

### 02: Data table and filters

The output should identify:

- Filter state, loading, apply/reset behaviour, and persistence expectations
- No-results and empty-data states
- Sort direction, active-sort indication, and persistence
- Wide-table strategy on small screens
- Long content, numeric alignment, and truncated data behaviour
- Save confirmation and repeat-save behaviour
- Keyboard interaction for filters, table rows, and row actions
- The unresolved purpose of row selection without a bulk action

It should not assume that all columns should be hidden on mobile.

### 03: Ambiguous confirmation modal

The output should rate the context as not ready.

It should identify:

- Destructive-action scope for collaborators and shared content
- Permission rules
- Whether recovery or a grace period exists
- Focus trapping, initial focus, Escape behaviour, and return focus
- Clear language naming what will be deleted
- The difference between deleting and leaving a shared workspace

It should not create a recovery policy that the product has not chosen.