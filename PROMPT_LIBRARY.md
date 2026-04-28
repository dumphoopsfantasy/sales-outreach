# PROMPT_LIBRARY.md

Reusable prompts for AI-assisted sales outreach. Every prompt here assumes the AI has read `CLAUDE.md` and `PERSONAS.md` first.

## How to use

1. Pick the prompt that matches your task.
2. Fill in the bracketed variables `[LIKE THIS]`.
3. Paste into Claude, Perplexity, or ChatGPT.
4. If the AI skips the success criteria, stop it and re-send.

---

## 1. Prospect Research Brief

Use before any first-touch outreach to a new account.
Read CLAUDE.md and PERSONAS.md before responding.

Research this prospect and return a brief:

Company: [COMPANY NAME]

Contact: [FIRST LAST], [TITLE]

Vertical: [HEALTHCARE / PHARMA / FINANCIAL SERVICES]

Return:

Likely persona match from PERSONAS.md (pick one, justify in 1 sentence)

One current business initiative (from news, press, LinkedIn, earnings, or site)

One likely application delivery or modernization pain

One specific, non-generic outreach hook tied to items 2 and 3

One disqualifier if present (wrong size, wrong stack, recent bad press)

Rules:

Do not invent facts.

Cite sources for items 2 and 3.

If information is thin, say so. Do not pad.

text

---

## 2. First-Touch Cold Email (3 Variants)

Use after running the research brief above.
Read CLAUDE.md and PERSONAS.md before responding.

Write 3 first-touch cold email variants for:

Persona: [PERSONA FROM PERSONAS.MD]

Company: [COMPANY NAME]

Hook: [HOOK FROM RESEARCH BRIEF]

Rules:

Max 80 words each.

One pain point, one proof point, one CTA.

No calendar links.

No "hope this finds you well."

One personalization variable maximum.

CTA must be low-friction (a question or a 15-min peer conversation).

Return:

Variant A: direct pain-led

Variant B: peer-story-led

Variant C: question-led

For each, add 1 sentence explaining why it should earn a reply.

text

---

## 3. Sequence Step Diagnostic

Use on any underperforming Apollo sequence before rewriting.
Read CLAUDE.md before responding.

Here is my current Apollo sequence:
[PASTE ALL STEPS]

Performance:

Delivered: [N]

Replies: [N]

Reply rate: [%]

Tasks:

Identify the SINGLE weakest step and explain why in 2 sentences.

Do NOT rewrite anything yet.

State 2 testable hypotheses for why this step is underperforming.

Propose the smallest possible change to test each hypothesis.

Rules:

Surgical only. One step.

No broad rewrites.

No new sequence structures.

text

---

## 4. Sequence Step Rewrite (Surgical)

Use only after running the diagnostic above.
Read CLAUDE.md and PERSONAS.md before responding.

Rewrite ONLY step [N] of this sequence. Leave all other steps unchanged.

Original step:
[PASTE STEP]

Persona: [PERSONA FROM PERSONAS.MD]
Goal of this step: [REPLY / BOOK CALL / RE-ENGAGE / BREAK UP]
Hypothesis being tested: [FROM DIAGNOSTIC]

Rules:

Max 80 words.

One clear CTA.

No calendar links.

Match tone of surrounding steps.

Do not change subject line unless the hypothesis specifically targets it.

Return:

The new step

1 sentence explaining how it tests the hypothesis

1 sentence explaining what reply rate would count as success

text

---

## 5. LinkedIn Connection + Follow-Up

Use for Day 1 LinkedIn engagement before the email sequence starts.
Read CLAUDE.md and PERSONAS.md before responding.

Write a LinkedIn connection request and a follow-up message for:

Persona: [PERSONA]

Company: [COMPANY]

Hook: [HOOK]

Connection request rules:

Max 280 characters.

No pitch.

One genuine reason to connect.

Follow-up message (sent 1 day after accept) rules:

Max 50 words.

Reference the hook.

Low-friction question, not a pitch.

No calendar link.

text

---

## 6. Competitive Positioning

Use when a prospect mentions Mendix, Microsoft Power Platform, or Salesforce Platform.
Read CLAUDE.md before responding.

A prospect is evaluating OutSystems vs. [COMPETITOR].

Persona: [PERSONA]
Stated priority: [SCALE / INTEGRATION / GOVERNANCE / DEV EXPERIENCE / COST]

Return:

3 honest tradeoffs (not marketing claims)

1 scenario where the competitor is the better fit

1 scenario where OutSystems + Noesis delivery is the better fit

1 question I should ask the prospect next to narrow the decision

Rules:

No invented benchmarks.

No superlatives.

Conservative, specific language only.

text

---

## 7. Break-Up Email

Use as the final step of any sequence with no reply.
Read CLAUDE.md before responding.

Write a break-up email for:

Persona: [PERSONA]

Company: [COMPANY]

Prior touches: [N]

Rules:

Max 50 words.

One question that gives them an easy out.

No guilt, no pressure, no "last chance" language.

No calendar link.

text

---

## 8. Post-Reply Response

Use when a prospect replies with interest, skepticism, or a brush-off.
Read CLAUDE.md and PERSONAS.md before responding.

The prospect replied:
[PASTE REPLY]

Classify the reply: INTEREST / OBJECTION / BRUSH-OFF / REFERRAL / NOT NOW.

Then write a response that:

Matches the classification.

Moves toward the next step (conversation, intro, or scheduled follow-up).

Stays under 60 words.

Does not pitch if the reply was a brush-off.

text

---

## 9. Loom Video Script

Use for Day 4 Loom video in the 4-day multi-channel framework.
Read CLAUDE.md and PERSONAS.md before responding.

Write a 60-second Loom video script for:

Persona: [PERSONA]

Company: [COMPANY]

Hook: [HOOK]

Structure:

0–10s: Their name, why I recorded this specifically for them

10–30s: The specific pain I believe they are facing and why

30–50s: One peer example or proof point

50–60s: One simple question, no pitch

Rules:

Conversational, not scripted.

No feature dumps.

No calendar link.

text

---

## 10. Weekly Sequence Review

Run every Friday against live Apollo data.
Read CLAUDE.md before responding.

Here is this week's Apollo data for sequence [NAME]:

Sent: [N]

Opens: [N] ([%])

Replies: [N] ([%])

Meetings booked: [N]

Return:

Which step is pulling the weakest (open or reply)?

Is the weakness at the top of funnel (subject line) or mid (body/CTA)?

One hypothesis to test next week.

The smallest possible change to test it.

Rules:

No broad rewrites.

No more than one change per week.

Preserve a control version.

text

---

## Control Discipline

Before any rewrite, save the current version in `sequences/` as:
`[sequence-name]_v[N]_[YYYY-MM-DD].md`

Never overwrite a live version without a dated backup.
