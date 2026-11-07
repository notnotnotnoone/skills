---
name: evaluate-app-idea
description: Skeptically evaluate whether a software or app idea deserves development using weighted gates, closest-substitute tests, and brutal economic reality checks. Use when a user pitches a product, asks whether an idea is worth building, wants competitor/substitute research, or requests an adversarial product review.
---

# Evaluate App Idea — Adversarial Review & Grading System

## Purpose

Act as an adversarial, research-driven review board for software and app ideas. Decide whether a proposed project deserves development time or if it should be killed immediately before a single line of code is written.

The core guiding principle is:
> **Every idea competes against current behavior and the closest mundane alternative (even the Apple Notes app, a spreadsheet, or doing nothing). If switching does not offer a massive, undeniable advantage over that baseline, users will never adopt it—and they will certainly never pay for it.**

Do not act as a startup cheerleader, feature brainstormer, or idea rationalizer. The default posture is skeptical: **attempt to disprove the case for building**.

---

## The 6 Hard Kill Switches (Fatal Overrides)

Before calculating numerical scores, test against the **6 Hard Kill Switches**. If any single switch trips, the verdict is an automatic **REJECT** or **PIVOT REQUIRED**, regardless of how high other criteria score.

1. **The Public Commodity Wrapper Trap:**
   * The app merely displays or organizes data that is already public, free, and better-served by dominant platforms (e.g., meme coin/crypto tickers, weather, public RSS, stock trackers, flight trackers). No proprietary data, no private signal.
2. **The "Notes App / Status Quo" Superiority:**
   * The closest mundane alternative (Apple Notes, a Google Doc, pen and paper, a group chat, or doing nothing) solves 80% of the practical need with 0% extra adoption friction. The friction of installing, setting up, and remembering a new app outweighs the minor convenience gained.
3. **The Marginal Switching Advantage (<2x):**
   * The product offers only incremental aesthetic or feature improvements (e.g. "a cleaner UI", "it has dark mode", "it uses AI"). If switching requires downloading an app, creating an account, or importing data for less than a dramatic improvement, users will churn in 48 hours.
4. **The Zero-WTP / Vanity Subscription Delusion:**
   * Asking users to pay \$5–\$20/month for a utility in a category where the industry standard is \$0 (ad-supported or platform-native), without generating measurable dollar ROI or preventing severe financial/legal loss.
5. **The Ghost Audience & Zero Distribution:**
   * The target audience is described vaguely as "everyone", "crypto traders", "students", or "freelancers", and the founder has no direct, warm access to 100+ members of this community. Relying on "posting on Twitter/TikTok" or "launching on Product Hunt" is an automatic failure.
6. **The AI/Tech Decorative Wrapper:**
   * An LLM or API is bolted onto a simple deterministic workflow where a simple filter, template, or manual check is cheaper, faster, and more reliable. The inference costs erode any realistic gross margin.

---

## The 5 Weighted Evaluation Gates (100-Point Quality Score)

Each gate is scored from **0 to 10 points** with explicit evidence-based justification, multiplied by its category weight to produce a final **Quality Score (0 to 100)**.

```
Total Quality Score = (Gate 1 × 2.5) + (Gate 2 × 3.0) + (Gate 3 × 2.0) + (Gate 4 × 1.5) + (Gate 5 × 1.0)
```

---

### Gate 1: Problem Reality & Pain Urgency (Weight: 25%)

Measures whether the problem exists in the real world and how badly the user wants it solved.

* **1.1 Acute Pain vs. Vitamin (0–10 pts):**
  * *10 = Emergency Room Pain:* Users actively lose money, hours of grueling work, or face legal/reputational disaster daily without a solution.
  * *5 = Annoying Friction:* Users complain when prompted, but tolerate the status quo for months without actively searching for a fix.
  * *0 = Made-Up Problem / Vitamin:* "Wouldn't it be cool if..." An app looking for a problem; nobody is actively suffering without it.
* **1.2 Target User & Workflow Specificity:**
  * Can the founder name the exact job title, the exact situational trigger, and the immediate preceding/following steps in their day?
* **1.3 Behavioral Evidence of Demand:**
  * Is there proof of existing workarounds, ugly hacky spreadsheets, money spent on kludged solutions, or repeated angry forum posts? (Compliments and survey "intent" count as 0).

---

### Gate 2: The Closest Substitute & Switching Advantage (Weight: 30%)
*(The Most Critical Gate — Where Most Apps Die)*

Measures the delta between the proposed product and the realistic alternative.

* **2.1 The "Closest Mundane Alternative" Baseline (0–10 pts):**
  * Identify what people *actually* do right now. Do not compare against a straw man. Look at:
    * The Apple Notes app / Google Keep
    * A shared Google Sheet / Excel
    * A Telegram / WhatsApp group or DM to self
    * A browser bookmark folder
    * Doing nothing / accepting the annoyance
  * If the closest option is free, instant, and frictionless, how heavy is the barrier to beat it?
* **2.2 The Direct Advantage & Switching Threshold (0–10 pts):**
  * *10 = 10x Direct Leap:* Cuts a 3-hour daily task to 3 minutes, makes users thousands of dollars, or unlocks an impossible capability. Switching is an absolute no-brainer.
  * *5 = 2x–3x Incremental Benefit:* Noticeably better, but requires onboarding friction, data migration, and habit re-learning. Many users try it and abandon it.
  * *0 = Marginal (<1.5x) or Pure Cosmetic:* "Better design," "All-in-one," or "Now with AI." The friction of switching dwarfs the benefit.
* **2.3 The Incumbent / Free Commodity Trap:**
  * Deep search for existing commercial products, open-source repositories, platform-native tools, or free web apps. If DexScreener, CoinGecko, or an Apple OS update can make this feature obsolete overnight, score is 0.

---

### Gate 3: Willingness-to-Pay (WTP) & Unit Economics (Weight: 20%)

Measures whether users will actually pull out a credit card and whether the business model is economically viable.

* **3.1 Economic Justification & Pricing Reality (0–10 pts):**
  * *10 = Obvious Financial ROI:* Charging \$50/mo to save \$500/mo in labor or recover \$2,000 in lost revenue. B2B corporate card expense.
  * *5 = High Consumer Delight:* Niche hobbyist with obsessive spending habits (e.g. vintage watch collectors, competitive powerlifters), but high churn risk.
  * *0 = The \$10/mo Delusion:* Charging a monthly fee for something consumers expect to be free, or where the utility delivered is worth pennies at best.
* **3.2 Margin & Cost-to-Serve:**
  * If the app uses third-party APIs (crypto node data, SMS, AI tokens), does heavy usage by a power user turn unit economics negative?

---

### Gate 4: Distribution & The First 10 Customers (Weight: 15%)

Measures whether the creator can actually get this in front of paying humans without paying for ads.

* **4.1 Day-1 Distribution Channel (0–10 pts):**
  * *10 = Unfair Proprietary Access:* The creator already runs an engaged community, newsletter, client roster, or Discord of 500+ exact target buyers.
  * *5 = Concentrated Watercooler:* The audience gathers in specific, identifiable subreddits, forums, or directories where high-signal manual outreach works.
  * *0 = Diffuse / Broadcast Praying:* Audience is scattered ("anyone who trades crypto"). The only distribution plan is "post on X", "make TikToks", or "launch on Product Hunt".
* **4.2 The "First 10 Customers This Week" Test:**
  * Can the founder manually contact and pitch 10 specific real people within 7 days without spending a dime on ads?

---

### Gate 5: Founder Wedge & Defensibility (Weight: 10%)

Measures why *this* founder can win and whether the app has any staying power.

* **5.1 Founder Wedge (0–10 pts):**
  * Does the founder have unique insider domain knowledge, a proprietary dataset, or deep technical capability that a random copycat lacks?
* **5.2 Defensibility & Copycat Ease:**
  * Could an experienced full-stack developer or an indie hacker replicate this app in 72 hours using Cursor or Antigravity? If yes, what prevents instant commoditization?

---

## Verdict & Quality Score Matrix

```
[Quality Score: 0 - 100]
85 – 100 : DEVELOP (Greenlit for 2-Week MVP)
65 – 84  : CONDITIONAL (Investigate / Pre-sale Test Required)
45 – 64  : PIVOT REQUIRED (Reposition to acute pain/B2B wedge)
 < 45    : REJECT (Dead on Arrival — Do Not Build)

*OVERRIDE RULE: If any of the 6 Hard Kill Switches trip, the verdict is REJECT regardless of score.
```

---

## Required Output Format

When invoked (via `$evaluate-app-idea [idea or pitch]`), produce an evidence-backed diagnostic report:

```markdown
# App Idea Evaluation: [Product Name / One-Liner]

## 1. Executive Verdict & Quality Score
* **Verdict:** [DEVELOP / CONDITIONAL / PIVOT REQUIRED / REJECT]
* **Quality Score:** [Score]/100
* **Fatal Overrides Tripped:** [None / Name of Kill Switch with 1-sentence proof]
* **The Bottom Line:** [1 brutal sentence explaining why this succeeds or dies]

---

## 2. The Core Assumption (BuilderOS Standard)
> "[The single statement that must be true for this business to survive. If false, the project is dead.]"

---

## 3. The Closest Substitute & Switching Analysis
* **The Closest Mundane Option:** [What users do right now — e.g. Apple Notes, spreadsheets, free DexScreener tabs, doing nothing]
* **The Incumbent / Free Landscape:** [Existing products, open-source projects, or free tools found during search]
* **The Switching Friction vs. Direct Advantage:** [Why users will or will not switch. Is the advantage 10x or <1.5x?]

---

## 4. The 5-Gate Scorecard

| Gate | Focus | Weight | Score (0–10) | Weighted | Brutal Diagnosis & Evidence |
| :--- | :--- | :---: | :---: | :---: | :--- |
| **Gate 1** | Problem Reality & Pain Urgency | 25% | _/10 | _/25 | [Specific evidence of pain/workaround] |
| **Gate 2** | Closest Substitute & Switching Leap | 30% | _/10 | _/30 | [Comparison against closest option] |
| **Gate 3** | Willingness to Pay & Economics | 20% | _/10 | _/20 | [ROI justification for pricing] |
| **Gate 4** | Distribution & First 10 Customers | 15% | _/10 | _/15 | [Direct channel reality check] |
| **Gate 5** | Founder Wedge & Defensibility | 10% | _/10 | _/10 | [Moat and copycat defense] |
| **TOTAL** | **Quality Score** | **100%** | | **_/100** | **[VERDICT]** |

---

## 5. Fatal Flaws & Red Flags (Max 3)
| Risk / Flaw | Severity | Why It Kills the Business | Cheap Behavioral Test to Verify |
| :--- | :--- | :--- | :--- |
| ... | High | ... | ... |

---

## 6. The Action Plan (If Not Rejected)
* **First 10 Customers Playbook:** 3 concrete manual outreach actions for this week.
* **2-Week MVP Test:**
  * **Build:** The minimum testable core.
  * **Cut:** Everything else (auth, settings, multi-tier billing).
  * **14-Day Validation Test:** Exact criteria for pass/fail.
```

---

## Calibration Benchmarks

### 1. The Meme Coin Tracker (The \$10/mo Commodity Delusion)
* **Pitch:** An app that tracks meme coin price movements, pumps, and liquidity, charging \$10/month.
* **Closest Substitute:** DexScreener, Birdeye, CoinGecko, Telegram alert bots, pump.fun terminal (all 100% free with massive server infrastructure).
* **Verdict:** **REJECT (Score: 18/100)**
* **Kill Switch Tripped:** *The Public Commodity Wrapper Trap* & *The Zero-WTP Delusion*. Zero proprietary signal, charging \$10/month for public API wrappers that free tools do 100x better.

### 2. The Custom Habit Tracker (The Apple Notes Trap)
* **Pitch:** A beautiful, minimal habit and routine tracker with streak animations for \$4.99/mo.
* **Closest Substitute:** Apple Notes bullet list, pen and paper, free default phone alarms, or existing free habit apps (Streaks, Habitica).
* **Verdict:** **REJECT (Score: 32/100)**
* **Kill Switch Tripped:** *The "Notes App / Status Quo" Superiority*. The switching friction of maintaining a dedicated app for daily micro-tasks leads to 90% churn in 30 days.

### 3. YC Classic: Carta (Replacing Cap Table Spreadsheets)
* **Pitch:** Software to track startup equity, cap tables, and investor options.
* **Closest Substitute:** A messy Excel file maintained by a lawyer at \$800/hour.
* **Verdict:** **DEVELOP (Score: 92/100)**
* **Analysis:** Bleeding-neck pain (costly legal mistakes, fundraising diligence chaos), massive financial ROI (saves thousands in legal fees), defensible network effects between companies and investors.
