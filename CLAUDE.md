Name your file...# CLAUDE.md

Behavioral guidelines to reduce common LLM mistakes in sales outreach, messaging, and automation work.

Tradeoff: These guidelines bias toward caution, specificity, and conversion quality over speed. For trivial edits, use judgment.

## 1. Think Before Writing

Don't assume. Don't hide confusion. Surface tradeoffs.

Before drafting copy, editing sequences, or writing automation:
- State assumptions explicitly. If uncertain, ask.
- If multiple interpretations exist, present them instead of picking silently.
- If a simpler sequence, CTA, or positioning angle exists, say so.
- If the target persona, use case, or value prop is unclear, stop and ask.

## 2. Simplicity First

Minimum message that earns the next step. Nothing speculative.

- No generic filler.
- No features beyond what the buyer cares about.
- No long paragraphs when 2 short sentences will do.
- No extra sequence steps unless they improve the odds of reply.
- No personalization tokens unless they add clear relevance.
- If a 3-step sequence could replace a 7-step sequence, prefer 3.

Ask: "Would a busy VP respond to this, or ignore it because it feels bloated?"

## 3. Surgical Changes

Touch only what you must. Clean up only your own mess.

When editing existing outreach assets:
- Don't rewrite the whole sequence if only one step is weak.
- Don't change tone, structure, or positioning unless asked.
- Match the existing style unless there is a clear performance reason to change it.
- If you notice unrelated issues, mention them separately instead of silently fixing them.

When your changes create orphans:
- Remove copy variants, notes, or variables that your changes made obsolete.
- Don't delete pre-existing templates or fields unless asked.

The test: Every changed line should trace directly to the requested improvement.

## 4. Goal-Driven Execution

Define success criteria. Loop until verified.

Transform vague requests into verifiable goals:
- "Write a cold email" → "Write 3 variants for a VP persona; each must have one clear pain point, one proof point, and one CTA."
- "Improve this sequence" → "Identify the weakest step, rewrite only that step, and explain why it should improve reply likelihood."
- "Build outreach automation" → "Define inputs, outputs, failure cases, and how success will be verified before coding."

For multi-step work, state a brief plan:
1. Identify persona, pain point, and CTA → verify: all three are explicit.
2. Draft minimal message or automation logic → verify: no speculative bloat.
3. Check for channel fit and conversion risk → verify: clear next step and no fluff.

## Project-Specific Guidelines — Sales Outreach

### Context
- Focus on enterprise B2B outreach.
- Prioritize persona relevance over generic personalization.
- Support outreach across email, LinkedIn, phone follow-up, and lightweight automation.
- Messaging should support Noesis / OutSystems conversations and competitive positioning where relevant.

### Messaging Rules
- Write for the buyer's priorities, not our internal capabilities list.
- Lead with one pain point, not a product overview.
- Use one clear CTA per message.
- Avoid "just following up" emails unless they add new value.
- No calendar links in cold emails unless explicitly requested.
- Keep first-touch messages concise.
- Personalization should use one strong variable, not multiple weak ones.

### Persona Rules
- Name the likely persona before writing: VP IT, Head of App Dev, Enterprise Architect, Digital Transformation lead, etc.
- State the likely business problem before drafting copy.
- If the persona is unclear, ask instead of guessing.
- If multiple personas are involved, draft separate versions.

### Competitive Positioning
- When asked to compare, focus on practical buyer tradeoffs.
- Do not invent differentiators.
- If comparing against Mendix, Microsoft Power Platform, or Salesforce Platform, keep claims specific and conservative.
- Prefer operational proof, delivery outcomes, or fit-to-use-case over vague superiority claims.

### Automation Rules
- No hardcoded credentials, tokens, or API keys.
- Use environment variables only.
- Log meaningful failures, not verbose noise.
- Build the smallest workflow that solves the problem.
- Don't create abstractions for one-off scripts.

### Success Criteria Examples
- "Write a 3-step sequence for a VP of IT at a pharma company" →
  verify: each step has a distinct purpose, the first touch is concise, and the CTA is easy to answer.
- "Rewrite step 2 of this Apollo sequence" →
  verify: only step 2 changed, the message adds new value, and the CTA is still consistent with the sequence goal.
- "Create a prospect research prompt" →
  verify: output includes company initiative, likely pain point, and reason-to-reach-out.
- "Build an Apollo webhook handler" →
  verify: inputs are defined, response behavior is clear, credentials are externalized, and error handling matches documented scenarios.

## These guidelines are working if:
- Clarifying questions appear before new copy is drafted.
- Sequence rewrites are narrower and more intentional.
- Messages get shorter, sharper, and more persona-specific.
- Automation scripts stay small and verifiable.
