# Agent playbooks

## How Makenna should work with agents

An agent is a temporary specialist, not an authority. Give it a narrow job, evidence rules, and a deliverable. Then check its work against primary sources and human interviews.

Use this pattern in every chat:

```text
You are my [ROLE] for a student research project. Our question is:
[QUESTION]

Your task: [ONE SPECIFIC JOB].
Audience: fitness-minded U.S. college students and 20-somethings.
Constraints: This is a concept, not a launched food product. Do not invent facts,
citations, suppliers, prices, test results, or legal conclusions. Flag uncertainty.
Use primary or clearly named sources and link every factual claim.

Output:
1. Findings (with source links)
2. Assumptions and unknowns
3. Contradictory evidence
4. Questions I should investigate with real people or professionals
5. A one-paragraph recommendation—clearly marked as your opinion
```

After every run, Makenna adds a short note: **What I accepted, what I rejected, why, and what I will test next.** Save a copy or link to the prompt and output in `evidence/agent-runs/`.

## The agent team

### 1. Research Agent

**Job:** Build the evidence base without drifting into vague trend talk.

**Use for:** competitors, category language, pricing, formats, consumer behavior, sourcing questions, food regulation questions to investigate.

**Prompt addition:**

```text
Make a comparison table. Separate verified facts, reasonable inferences, and ideas.
Prioritize company sites, product labels, regulators, and credible original research.
For each gap, tell me exactly how I could verify it.
```

**Quality check:** Open three source links yourself. Ask: is the fact current? does it apply to this exact product/market? is an inference being presented as fact?

### 2. Interview Coach

**Job:** Help design unbiased conversations and turn notes into insights.

**Use for:** interview guide, recruitment message, follow-up questions, anonymized note coding.

**Prompt addition:**

```text
Do not ask people to predict whether they would buy my idea. Help me learn about
their actual recent behavior, choices, budget, routines, and frustrations. Flag
leading questions and suggest neutral replacements.
```

**Quality check:** Interviews should include direct quotes, observed patterns, and contradictions—not just counts.

### 3. Strategy Agent

**Job:** Turn evidence into several sharply different choices.

**Use for:** segment definition, jobs-to-be-done, positioning territories, reasons to believe, brand architecture.

**Prompt addition:**

```text
Develop 3 distinct territories. For each, write: target customer, tension,
category frame, promise, reasons to believe, personality, exclusion, and the
evidence it relies on. Avoid health or performance claims unless proven for the
exact product.
```

**Quality check:** Makenna must be able to explain each choice in plain English, without design language.

### 4. Skeptic Agent

**Job:** Attack the strongest idea before the market does.

**Use for:** every major gate, price/format assumptions, credibility, cultural fit, competitor response, risks.

**Prompt addition:**

```text
Assume this concept fails. Give me the 10 most likely reasons, ranked by severity
and likelihood. Identify what evidence would reduce each uncertainty. Do not be
nice; be specific and fair.
```

**Quality check:** A good critique produces a next test or a clear no-go—not defensiveness.

### 5. Claims Auditor

**Job:** Catch words that create factual promises.

**Use for:** product pages, labels, social captions, creator briefs, comparisons.

**Prompt addition:**

```text
Extract every explicit and implied product, nutrition, health, performance,
sourcing, sustainability, safety, and comparative claim. Put each in a table
with consumer interpretation, evidence needed, risk level, and a safer temporary
alternative. Do not approve claims or give legal advice.
```

**Quality check:** Put every flagged term in the claim register. Approval belongs to qualified people, not an agent.

### 6. Creative Assistant

**Job:** Explore visual and verbal systems after strategy approval.

**Use for:** name directions, tone of voice, creative brief, moodboard vocabulary, package and content concepts.

**Prompt addition:**

```text
Create three coherent territories, not a pile of logos. For each, state the
strategic idea, visual grammar, verbal voice, distinctive assets, risks, and what
it must not resemble. Do not copy living brands, artists, or designers.
```

**Quality check:** Show a generic, unbranded version of the work to participants. If they cannot describe the intended feeling/offer, the system is not doing its job.

### 7. Brand QA Agent

**Job:** Check consistency against the approved strategy.

**Use for:** product page, email, paid ad, package, social post, future category idea.

**Prompt addition:**

```text
Compare this artifact with the approved strategy and claims boundaries. Identify
inconsistencies, unsupported promises, accessibility/readability issues, and
places where the work looks generic. Give revisions in priority order.
```

### 8. Experiment Designer

**Job:** Make a test capable of changing Makenna's mind.

**Use for:** concept cards, website usability, price/pack tests, marketing messages.

**Prompt addition:**

```text
Create a small, ethical research test with a hypothesis, audience, stimulus,
neutral questions, comparison/control, success threshold, failure threshold,
biases, and analysis plan. Do not present a concept test as product validation.
```

## The required reflection: Where AI was wrong

At the end of every phase, complete this four-line entry:

```text
AI predicted:
Evidence showed:
My decision:
What I changed in the next prompt or test:
```

This is one of the most valuable parts of the eventual portfolio. It shows Makenna's judgment rather than merely her ability to generate output.
