## Purpose

A decision tool for choosing which research approach to emphasize at any given moment. Four concurrent lenses—Discovery, User Testing, Feedback, Experimentation—each answering a different core question. Not sequential phases; all four apply throughout product work. Informed by Christian Rohrer's [Landscape of User Research Methods](https://www.nngroup.com/articles/which-ux-research-methods/) (NN/g), which maps 20 UX research methods across three dimensions: attitudinal vs. behavioral, qualitative vs. quantitative, and context of product use.

This framework is not necessarily aligned with other major product and product research experts in the industry (Teresa Torres, Marty Cagan/SVPG, Tim Herbig, Eric Ries, etc.). Standardizing on one coherent body of work keeps gate criteria, lens taxonomy, sample-size guidance, and interview craft built on shared assumptions—mixing frameworks tends to break that consistency at the seams, and a single methodology produces faster, more legible plans across the team.

Nielsen Norman Group is that body of work. Before proposing a methodology change—interview structure, usability protocol, sample size, a new template section—check NN/g's current guidance and cite the specific article rather than improvising from intuition or general practice.


---

## The Four Lenses

### 1. Discovery

*"Are we solving the right problem?"*

Grounds the team in the user's actual work, decisions, and context before designing solutions. Observes behavior and surfaces unmet needs.

- **Focus areas:** What users actually do, what needs are unmet, whether the project is worth doing
- **Typical methods:** User interviews, field studies, diary studies, contextual inquiry, competitive analysis
- **Delivers:** Problem statement (qualitative, generative)
- **Addresses risk:** Value, viability
- **Rohrer dimensions:** Primarily behavioral and qualitative, natural or near-natural context of use
- **Typical participants:** At least 5 per persona per NN/g; continue until saturation.
- **Typical duration:** 2–4 weeks end-to-end.
- **Templates:** [Discovery](Discovery/Discovery.md) (plan) · [Discovery Results](Discovery/Discovery%20Results.md)

### 2. User Testing

*"Can people actually use this?"*

Observes real people interacting with a design or prototype to identify usability problems before launch.

- **Focus areas:** Where people get confused, why they abandon tasks, what the design gets wrong
- **Typical methods:** Think-aloud tests, task scenarios, moderated and unmoderated remote testing, usability benchmarking
- **Delivers:** Usability fixes (behavioral, evaluative)
- **Addresses risk:** Usability, value
- **Rohrer dimensions:** Behavioral, qualitative, scripted or limited context of use
- **Typical participants:** 5 per persona per [NN/g's 5-user rule](https://www.nngroup.com/articles/why-you-only-need-to-test-with-5-users/) (catches ~85% of usability problems)—the default. Quantitative benchmarking is a specialized case requiring 20–40 total for statistical metrics; use sparingly.
- **Typical duration:** 1–2 weeks per round.
- **Templates:** [User Test](User%20Test/User%20Test.md) (plan) · [User Test Results](User%20Test/User%20Test%20Results.md)

### 3. Feedback

*"What do users say they think and want?"*

Collects self-reported attitudes and reactions at any stage of product work—post-launch, mid-beta, or concept phase.

- **Focus areas:** Self-reported attitudes and reactions, stated pain points and desires, satisfaction and sentiment trends
- **Typical methods:** Surveys, NPS/CSAT, concept tests, beta feedback, support logs, product reviews, feedback interviews
- **Delivers:** Sentiment signal (attitudinal, continuous)
- **Addresses risk:** Value, viability
- **Rohrer dimensions:** Attitudinal, mixed qualitative and quantitative, decontextualized
- **Typical participants:** At least 5 per persona for qualitative interviews; continue until saturation. ~40 minimum for surveys.
- **Typical duration:** 1–3 weeks depending on instrument.
- **Templates:** [Feedback](Feedback/Feedback.md) (plan) · [Feedback Results](Feedback/Feedback%20Results.md)

### 4. Experimentation

*"Which option performs better?"*

Measures which design option performs better with live users, using controlled comparison.

- **Focus areas:** Which variant moves the metric, statistical significance of a change, measurable impact on business KPIs
- **Typical methods:** A/B testing, multivariate testing, feature flags, holdout experiments
- **Delivers:** Winning variant (quantitative, evaluative)
- **Addresses risk:** Value, feasibility
- **Rohrer dimensions:** Behavioral, quantitative, natural context of use
- **Rigor framework:** Drawn from Ron Kohavi's *Trustworthy Online Controlled Experiments* (2020), since NN/g's guidance on experimentation focuses on the role of A/B testing alongside UX research rather than the statistical methodology (hypothesis format, primary vs. guardrail metrics, sample-size calculation, decision rule)
- **Typical participants:** Calculated from baseline metric, minimum detectable effect, and significance threshold.
- **Typical duration:** 1–2 weeks minimum to absorb day-of-week variance.
- **Templates:** [Experiment](Experiment/Experiment.md) (plan) · [Experiment Results](Experiment/Experiment%20Results.md)


---

## Is Research Warranted?

Not every question benefits from dedicated research. Apply this gate before committing a team to a study.

**Research is warranted when:**

- A specific decision is blocked by an unknown about users, behavior, or attitudes
- Stakeholders disagree on an assumption that new evidence could settle
- The cost of being wrong exceeds the cost of the research
- Existing data (analytics, support, prior studies) doesn't answer the question

**Research is probably not warranted when:**

- The decision is low-stakes and reversible—ship and learn is cheaper
- The question is already answered by existing signal (analytics, prior research, support logs, well-documented UX heuristics)
- The question asks users to predict their own future behavior—notoriously unreliable
- There's no actionable decision on the line—research for its own sake
- The answer is known; people want research to ratify a foregone conclusion


---

## Choosing a Lens

The question you're trying to answer determines the lens, not the method or instrument.

- **Use Discovery when:** You don't yet know what problem to solve, or you need to understand user context before designing. Example intents: "We're considering building X but don't know if users actually need it." / "We need to understand how [persona] makes decisions before designing the workflow."
- **Use User Testing when:** You have a design or prototype and need to find where it breaks before shipping. Example intents: "We have a mockup—can people actually complete the core tasks?" / "This flow feels confusing; where do users get stuck?"
- **Use Feedback when:** The product or feature is being used and you want to know how users feel about it, or what they want next. Example intents: "What do customers think of the new dashboard?" / "Which pain points come up most often in support?"
- **Use Experimentation when:** You have two or more specific design options and want to know which performs better on a metric. Example intents: "Does variant A convert better than variant B?" / "Will the new CTA increase signups?"

If the intent doesn't map cleanly, ask: "What decision will this research inform?" and pick the lens that answers that decision most directly. If still unclear, Discovery is the safe default—understanding is rarely wasted.


---

## Key Distinctions

### Discovery vs. Feedback

Both can use interviews as a method, but the target signal differs. [Attitudinal vs. Behavioral Research in UX](https://www.nngroup.com/articles/attitudinal-behavioral/) (NN/g) defines the split as self-report versus observation.

- **Discovery** observes behavior and probes the user's world without requiring product context. The question is "what problems do you have?"—product may not come up at all.
- **Feedback** collects self-reports anchored to a product. The question is "what do you think about X, how does X serve you, what do you want from X?"

Feedback interviews still use behavioral anchoring (critical-incident technique, "walk me through the last time you used X") to reduce recall bias and ground self-report. The behavioral anchor is technique; the target is attitudes, reactions, and stated desires. Don't let the "Feedback = self-report" framing push concrete-event questions into Discovery where they don't belong.

### User Testing vs. Experimentation

Both observe behavior, but differ in method and scale.

- **User Testing** is qualitative and moderated (or unmoderated with small N). Typically five to eight participants, observing behavior in context of use. Outputs are usability issues and friction points.
- **Experimentation** is quantitative and at scale. Typically thousands of participants via A/B split. Outputs are conversion or engagement metrics.


---

## Common Mistake

Treating the four lenses as sequential phases instead of concurrent lenses. Strong teams apply all four continuously—choosing which to emphasize based on the biggest uncertainty right now. Teams that skip Discovery succeed at barely better than chance. Teams that run experiments without first understanding the problem optimize the wrong thing.


---

## Vocabulary

NN/g terms the templates depend on:

- **Interview guide**: A semistructured, flexible instrument. This is what the templates produce.
- **Interview script**: A structured, rigid instrument. Not what we write—the distinction matters when someone asks for a "script."
- **Research questions**: Study-level objectives. Distinct from interview questions, which are the elicitation prompts that answer them.
- **Funnel technique**: Ordering questions broad to specific.
- **Probes and follow-ups**: Sub-questions for drilling into an answer.

NN/g does not use named phase sections—no Warmup, Main Questions, Reflection, or Closing headings. The interview guide is a flat numbered list where structure is encoded by position. The Discovery, Feedback, and User Test templates follow this: a single `## Questions` section, flat numbered list, probes as sub-bullets.

Reference articles: [Writing an Effective Guide for a UX Interview](https://www.nngroup.com/articles/interview-guide/), [User Interviews 101](https://www.nngroup.com/articles/user-interviews/), and the [Example Guide for a Semistructured Interview](https://media.nngroup.com/media/articles/attachments/example_interview_guide.pdf) (PDF).


---

## Research Template Conventions

Research templates and results docs follow vault-wide conventions in AGENTS.md with these specific exceptions for cross-surface compatibility with the GitHub mirror at `designerdean-rentable/aiq-research-mirror`:

- **H3 (`###`) is allowed** within H2 sections, unlike the rest of the vault (which skips H3 in favor of H4). H3 renders cleanly on the GitHub mirror.
- **Placeholders use bracketed text** (e.g., `[Observation]`, `[Takeaway]`) for team-facing clarity, rather than the empty-bullet placeholders used elsewhere in the vault.
- **Callouts are authored Obsidian-style**: marker and custom title on the same line (`> [!note] Title`). The mirror workflow at `.github/workflows/mirror-aiq-research.yml` reformats these to GitHub's alert syntax on sync (marker on its own line, custom title bolded on the next).

Two further conventions, both about keeping concerns on the right surface:

- **Research questions stay persona-agnostic.** Questions express what you are trying to learn; the participant list says who you are learning it from. Naming personas inside questions creates false contrast—it reads as though some questions are persona-differentiated when all are cross-persona. Group participants under persona subheads instead, and coverage becomes self-documenting.
- **Per-session scaffolding holds only recurring work.** Pre-Interview Tasks, Pre-Test Tasks, and Introduction bullets are prep that happens before *every* session. One-time study setup—piloting the guide, defining the outreach list, drafting the script, getting CS or sales intros—belongs at the study-plan level. Before adding an item, ask whether it happens every session or once per study.
