# Evaluation criteria

Use these criteria to assess whether the output is specific, proportionate, and useful.

## It must

- Identify the actual user decision or workflow the AI feature affects.
- Question whether AI is necessary when simpler approaches could solve the stated problem.
- Distinguish assistance, recommendation, confirmation-based action, and automation.
- Tie each risk to a specific failure mode in the supplied concept.
- Recommend proportionate safeguards, not vague assurances.
- Identify when users need sources, provenance, freshness, limitations, or uncertainty to judge an output.
- Consider reversibility, user control, and safe failure states.
- Avoid claiming legal, security, regulatory, or compliance certainty without supplied evidence.
- Recommend one concrete next step before delivery.

## It must not

- Produce a generic list of “AI risks” without connecting them to the feature.
- Assume a confidence score makes an output trustworthy or understandable.
- Treat competitor activity as evidence that customers need the feature.
- Recommend automation by default.
- Invent model capabilities, technical controls, policies, laws, or user research.
- Over-escalate low-stakes AI assistance into a high-risk scenario without justification.
- Underestimate higher-stakes use cases merely because a human is technically “in the loop.”

## Expected behaviour by example

### 01: Research Answer Assistant

The output should assess this as generally low-to-medium risk, depending on how the answers are used.

It should identify:

- The need for source citations and direct links to underlying research
- Permissions enforcement across retrieved content
- Freshness, date context, and coverage gaps
- Clear distinction between sourced evidence and generated synthesis
- A safe response when the system lacks reliable evidence or sources conflict

It should not treat a generic confidence score as sufficient transparency.

### 02: Support Ticket Triage

The output should assess this as medium risk because the feature affects customer response quality, operational priorities, and potentially sensitive or security-related information.

It should identify:

- The need for agent review and easy correction
- Risks of under-prioritising urgent, security, or vulnerable-customer cases
- Sensitive-data handling in ticket content
- Monitoring of override rates, misroutes, and category-level error patterns
- A clear escalation route for security incidents

It should recognise that a reversible suggestion is safer than automatic routing, but not risk-free.

### 03: Portfolio-Rebalancing Recommendations

The output should assess this as high risk.

It should identify:

- The distinction between financial education, personalised recommendation, and automated action
- The need to examine applicable regulatory and compliance obligations before design
- Data freshness, customer suitability, explainability, and auditability
- The risk that users interpret recommendations as guaranteed or authoritative
- Strong user review, explicit confirmation, and safe restrictions around automatic trades
- The weak relationship between “assets under management” and positive customer outcomes

The recommended next step should be targeted problem validation plus specialist compliance/legal review before recommendation or automation design begins.