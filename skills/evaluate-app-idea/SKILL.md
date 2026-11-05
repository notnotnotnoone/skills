---
name: evaluate-app-idea
description: Skeptically evaluate whether a software or app idea deserves development. Use when a user pitches a product, asks whether an idea is worth building, wants competitor research, or requests an adversarial product review.
---

# App Idea Review

## Purpose

Act as a skeptical, research-driven review board for software and app ideas. Decide whether the proposed project deserves the user's development time. Do not act as a startup cheerleader, feature brainstormer, or idea validator.

The central question is:

**What valuable thing can a specific user do with this product that they cannot already do conveniently, and is that improvement worth the total cost of building and adopting it?**

The default posture is skeptical. Try to disprove the case for building. Do not rationalize weak ideas, invent a more attractive target audience, or add features to rescue a failed pitch unless the user explicitly asks to pivot.

A real problem does not automatically justify a standalone product. A novel implementation does not automatically create demand. A technically impressive demo does not automatically make a useful product.

## Invocation and inputs

Invoke as $evaluate-app-idea followed by the idea or pitch.

Start with the information already supplied. Do not make the user complete a long questionnaire. If one missing fact blocks meaningful evaluation, ask one focused question. Otherwise state assumptions and proceed.

Establish, as far as possible:

- The product's core job and intended outcome.
- The specific user and situation.
- The current workflow and workaround.
- The claimed advantage over alternatives.
- Whether the user wants a personal project, a commercial product, or both.
- The user's relevant building, debugging, and verification ability, time, budget, platform access, and tolerance for maintenance.

Do not assume the person evaluating the skill has the same skill level, resources, or goals as the original author. Ask or infer cautiously from explicit context, and label assumptions.

## The 32 evaluation criteria

Assess every criterion. Use Pass, Concern, Fail, or Unknown, with a short evidence-based explanation. A criterion is not a pass merely because no contrary evidence was found.

### Problem and demand

1. **Concrete problem and outcome.** Define the actual problem and the result the product is supposed to produce. Avoid vague categories such as "a better productivity app."
2. **Reality of the problem.** Find evidence that people experience this problem. Separate observed demand, user reports, and measured behavior from assumptions and hypothetical use cases.
3. **Frequency and severity of the actual failure.** Measure how often the specific problem or failure occurs, and how costly it is. Do not substitute the frequency of the surrounding activity. Uploading files daily does not mean selecting the wrong file happens daily. Rare events may still matter when consequences are severe.
4. **Specific users.** Identify who experiences the problem, in what context, and why they are a plausible user. "Everyone" is not a target audience.
5. **Evidence of demand.** Look for complaints, repeated workarounds, requests, spending, adoption, community discussion, or other behavioral evidence. A large theoretical audience is not proof of demand.

### Alternatives and competition

6. **Direct competitors.** Search deeply for products that solve the same job, including obscure GitHub repositories, indie apps, startups, research projects, abandoned products, plugins, browser extensions, and small commercial tools.
7. **Adjacent and built-in alternatives.** Investigate operating-system features, platform-native functions, existing app features, scripts, plugins, spreadsheets, command-line tools, and ordinary workflows that may solve enough of the problem.
8. **Strongest-alternative comparison.** Compare the proposed product against the strongest real substitute on the same concrete task. Do not choose a deliberately inconvenient straw-man workaround.
9. **ChatGPT and general AI substitution.** Ask whether a user can already get the outcome conveniently by asking ChatGPT or another general AI tool, including with a short prompt or uploaded file. Identify what requires persistent integration, local access, automation, or state that a normal chat cannot provide.
10. **Disposable solution test.** Could the user solve this with a tiny script, a coding agent, an internal tool, or a one-off automation in minutes? Compare the proposed product with the cheapest adequate solution, including its reliability and maintenance.
11. **Manual-work test.** Could a person simply perform the task manually in a few minutes? Count the actual steps and time. Do not invent an elaborate workaround when a quick check is adequate.
12. **Adoption effort.** Include discovery, trust, download, installation, setup, permissions, configuration, learning, migration, and ongoing maintenance. The benefit must justify the friction of adding another tool.

### Advantage and novelty

13. **Meaningful advantage.** Identify a concrete improvement in effort, quality, speed, cost, privacy, reliability, accessibility, or capability. "Cleaner UI," "uses AI," and "has more features" are not sufficient without a useful consequence.
14. **Reason to switch or add a tool.** Explain why the user would change an existing workflow or install another product. The advantage must outweigh switching and adoption costs.
15. **Crowding by functional overlap.** Judge the market by what products actually do, not just their names, categories, star counts, or marketing language. A small project may be a direct equivalent; a popular project may only be adjacent.
16. **Honest novelty classification.** Classify the idea as an existing equivalent, incremental improvement, meaningful combination, or substantially new approach. Do not call an idea novel because its exact name or wording is unfamiliar.
17. **Useful combination test.** A combination of features only counts as an advantage when their integration enables a meaningfully better workflow or outcome. Merely bundling familiar features is not novelty.

### Technology and economics

18. **AI necessity.** Decide whether AI is necessary, useful but optional, or decorative. Prefer deterministic or local methods when they deliver the same result more reliably or cheaply.
19. **Inference economics.** If AI is used, estimate realistic cost per user and at plausible usage levels. Consider input and output tokens, context size, request frequency, retries, caching, model choice, and heavy users. Compare cost with the value created and plausible pricing or budget.
20. **Latency.** Assess response time against the actual interaction. Consider time to first token, total completion time, network overhead, retries, and whether the user must wait or can work asynchronously.
21. **Hardest technical assumption.** Identify the assumption most likely to break the product. Distinguish a convincing demo from a dependable implementation.
22. **Reliability and maintenance.** Examine edge cases, integrations, platform restrictions, permissions, APIs, dependencies, data formats, compatibility, security, support burden, and ongoing maintenance.
23. **Builder fit.** Assess whether this particular user can realistically build, debug, test, and verify the core advantage with their actual skills and resources. Vibe-coded code that the builder cannot understand or validate is a risk. Flag specialist engineering requirements plainly.

### Scope, viability, and decision quality

24. **Audience sufficiency.** Decide whether the group that experiences the problem frequently enough is large or reachable enough for the user's goal. A niche is not automatically bad, but "some specialist might need this" is not evidence of a viable audience.
25. **Defensibility.** Assess honestly what would stop an existing product or another developer from copying the feature. Do not demand a venture-scale moat from a personal utility, but do not pretend a copyable feature is defensible.
26. **Distribution.** Identify a credible way to reach the intended users. Name actual channels and explain why those users would discover and trust the product. A theoretical app-store listing is not a distribution strategy.
27. **Personal and commercial value separately.** Give separate judgments for (a) whether it is worth this user's development time as a personal/learning project and (b) whether it has commercial potential, when both are relevant. A project can be personally worthwhile without being a business, or commercially interesting but a poor fit for this builder.
28. **Fatal weaknesses override strengths.** Do not average away a decisive flaw. A close existing equivalent, trivial workaround, negligible frequency, unjustifiable adoption cost, infeasible core assumption, or lack of meaningful advantage can override strengths elsewhere.
29. **Uncertainty and confidence.** State what is known, inferred, and unknown. Explain confidence and identify which missing evidence could change the verdict. Absence of search results is not proof that nothing exists.
30. **Cheapest decisive test.** Recommend the smallest, cheapest experiment that could resolve the most important uncertainty before substantial development. Examples include a targeted competitor search, a few user interviews, a landing-page test, a manual concierge test, a throwaway prototype, or measuring a real workflow.

### Two explicit cross-cutting rejection rules

31. **Total expected benefit must justify both sides' effort.** Evaluate the expected value against both user adoption effort and developer effort. For users, include finding, installing, configuring, learning, using, and maintaining the product. For the developer, include building, validating, distributing, supporting, and maintaining it. A product can save users a little time and still be a bad use of the developer's weeks. A useful estimate is: expected benefit = incident frequency × consequence per incident × proportion prevented, adjusted for realistic adoption and reachable users. Rare events can justify a product if consequences are severe; minor annual inconveniences usually cannot.
32. **Check the trivial built-in action before proposing automation.** Walk through the existing workflow and check for a normal button, setting, shortcut, confirmation, or built-in feature that already solves the problem adequately. If "Save As → Replace" solves it, do not pitch a download manager unless repeated, substantial savings are demonstrated.

## Research standard

Research is mandatory before any Develop verdict and before presenting a candidate idea as if it has survived inspection.

Search using multiple formulations:
- The problem described in the user's language.
- The user's workflow and desired outcome.
- Feature combinations and technical terms.
- Synonyms, adjacent categories, and alternative approaches.
- Names of likely products, projects, APIs, and relevant communities.

Investigate more than search-result titles. When relevant, inspect product documentation, demos, pricing, changelogs, release history, GitHub source, issues, discussions, screenshots, and actual workflows. Determine whether a competitor is functionally equivalent, partially overlapping, or merely adjacent.

Include:
- Mainstream commercial products.
- Small indie products and browser extensions.
- GitHub repositories, including low-star and abandoned projects.
- Startups and products with limited visibility.
- Research prototypes and academic work when relevant.
- Built-in platform features and ordinary tools.
- Scripts and workflows that users can create themselves.

Follow promising leads until the functional overlap is clear. Search until additional searches stop materially changing the competitive picture, and report important gaps. Do not claim that no competitor exists based on a few searches.

For each important alternative, report:
- Name and source link.
- What it actually does.
- The overlap with the proposed idea.
- Important differences or missing capabilities.
- Evidence quality and recency.
- Whether it is a direct equivalent, partial substitute, or adjacent tool.

Cite sources next to factual claims. Prefer primary sources for product capabilities and repositories. Use user discussions and reviews as evidence of experience or demand, not as unquestionable fact. Do not fabricate sources, product capabilities, adoption figures, or market sizes.

## Staged workflow

### Stage 1: Lead review and quick rejection screen

The lead reviewer frames the product and applies the obvious kill tests before expensive research:

- Is the problem concrete?
- Does the specific failure happen often enough or have severe enough consequences?
- Is there already a close equivalent?
- Is the current workaround trivial?
- Could a tiny script, coding agent, or manual action solve it adequately?
- Would users install and maintain another tool for this benefit?
- Is the core idea technically plausible for this builder?

If a decisive failure is already established, return Reject with evidence. Do not launch a theatrical multi-agent review to rediscover an obvious answer. If the idea is not yet rejectable, continue.

### Stage 2: Evidence-based investigation

Conduct the full competitor and alternative research. Complete all 32 criteria. Research the strongest substitutes before claiming differentiation.

If the idea fails, explain why and stop. Do not add speculative features or invent a different audience to rescue it. If a specific uncertainty is the only blocker, use Investigate further or recommend a narrowly scoped prototype.

### Stage 3: Independent sub-agent review for surviving ideas

Use sub-agents only when the idea survives the quick screen and independent work can add evidence. Keep the initial reviews independent. Do not prime agents with another reviewer's conclusion.

Use these roles when the environment supports sub-agents:

1. **Competitor investigator:** Search independently for direct and adjacent alternatives, including obscure repositories, indie apps, abandoned products, research, and built-in functionality. Report evidence and functional overlap.
2. **Adversarial reviewer:** Try to kill the idea. Challenge problem frequency, demand, adoption effort, trivial workarounds, claimed advantage, switching, distribution, and unsupported assumptions.
3. **Technical/economics specialist (conditional):** Add only when the main uncertainty involves difficult engineering, platform integration, reliability, AI inference cost, or latency.

The lead reviewer reconciles the findings and checks sources. No voting, majority rule, or consensus theater. Three agents agreeing is not proof. Conflicting claims must be investigated or reported as unresolved.

If sub-agents are unavailable, perform the roles as separate analytical passes and clearly state that no independent agents were actually run. Never claim to have launched agents when the environment did not support it.

### Stage 4: Final decision

Choose exactly one primary verdict:

- **Reject:** The idea does not justify development under the stated goal and evidence.
- **Investigate further:** A potentially important uncertainty remains; more evidence is needed before committing.
- **Prototype:** The idea has a plausible advantage, but a narrow experiment is needed to validate its hardest assumption.
- **Develop:** The evidence supports investing in a real implementation.

A Develop verdict requires a specific, defensible advantage, credible demand, adequate differentiation from alternatives, acceptable adoption and development costs, and feasible execution. Do not issue it while major competitor research is incomplete.

A project may receive different personal-project and commercial verdicts. State both when relevant.

## Calibration examples from the original design

Use these as reasoning examples, not as predetermined conclusions or current competitor research.

### Typer / Completionist

The original author considered Typer interesting because it appeared to combine system-wide Windows candidate autocomplete, local word ranking, AI phrase completion, and Text Services Framework (TSF) integration in an unusual way. Treat that combination as a hypothesis worth investigating. The combination matters only if it creates a user-visible advantage, and the technical complexity must be weighed against the builder's ability to debug and verify it.

### Flexrouter

The original author became much less interested in Flexrouter after discovering a mature project with roughly 77,000 stars and dozens of contributors that solved essentially the same problem. The lesson is not that star count alone decides the issue. The lesson is to discover mature functional equivalents early and determine whether the proposed product has a meaningful advantage.

### Windows text-input compatibility debugger

A proposed diagnostic tool for developers building text-input integrations sounded technically interesting, but the target audience was extremely niche and the workflow might be solved by testing a few apps or building a quick internal diagnostic. It was rejected for the original builder because the problem was too specialized and the required engineering was a poor fit. General rule: a real problem does not automatically justify a standalone product.

### Attachment mistake guard

A browser extension that warns when a user attaches an older copy of a document sounded plausible, but the actual mistake might happen only once a year. The setup and installation effort outweighed the expected benefit for a minor, rare failure. General rule: measure the frequency of the actual failure, not the surrounding activity.

### Repeated-download updater

A tool that routes repeated exports into a designated file sounded useful until the simple built-in Save As → Replace workflow was considered. General rule: compare against the actual easiest action, not an unnecessarily cumbersome workaround.

### AI feedback linked to document versions

A browser extension that linked AI review comments to the exact document version sounded plausible, but the user immediately identified that the capability already existed. General rule: research before presenting a candidate as novel, and require a meaningful advantage over existing equivalents.

## Required output format

Keep the report direct and evidence-heavy. Do not bury the verdict in a long generic essay.

1. **Verdict:** One of Reject / Investigate further / Prototype / Develop.
2. **One-sentence decision:** Why it does or does not deserve development.
3. **Idea as understood:** User, problem, workflow, product, and claimed advantage. List assumptions.
4. **Strongest case for it:** Best evidence supporting demand and advantage.
5. **Strongest case against it:** The most serious rejection argument.
6. **Competitor and substitute landscape:** Direct equivalents, partial substitutes, adjacent tools, built-in actions, ChatGPT/general AI, disposable scripts, and manual workarounds. Cite sources.
7. **32-criterion assessment:** A compact table with criterion, status, and evidence/reason. Do not omit criteria. Use Unknown rather than inventing a pass.
8. **Technical and economic assessment:** Hardest assumption, feasibility for this builder, reliability, AI necessity, cost, and latency where relevant.
9. **Sub-agent findings:** Separate independent findings and unresolved conflicts, or explicitly state that sub-agents were unavailable/not used.
10. **What would change the verdict:** Specific evidence or conditions, not vague optimism.
11. **Cheapest decisive next test:** One practical test with a clear success/failure condition.
12. **Final rationale:** If recommending development, complete this sentence: "Build this because [specific users] repeatedly need [outcome], and existing options fail at [important limitation]." If that sentence cannot be supported, do not give a Develop verdict.

## Behavioral constraints

- Do not flatter the idea or the user.
- Do not invent demand, competitors, metrics, citations, or technical certainty.
- Do not treat a lack of search results as proof of novelty.
- Do not equate GitHub stars with functional equivalence or product quality.
- Do not count surrounding activity as evidence that the failure itself is frequent.
- Do not compare against an artificially inconvenient workaround.
- Do not recommend a product when a built-in action is already adequate.
- Do not rescue a failed pitch by adding features or changing audiences without explicit permission.
- Do not let a numerical score, average, or agent consensus override a fatal weakness.
- Do not fabricate a weighted score. The source design specifies categorical judgments and verdict logic, not a validated numerical weighting formula.
- Distinguish facts, estimates, assumptions, and hypotheses.
- Preserve user agency: give a reasoned recommendation, not a command.
