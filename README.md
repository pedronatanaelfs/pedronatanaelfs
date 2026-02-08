# Hi, I’m Pedro Silva
Data Scientist focused on gaming analytics: gameplay insights, retention, monetization, experimentation, and player voice.

Location: Brazil  
Email: pedronatanaelfs@gmail.com  
LinkedIn: https://www.linkedin.com/in/pedro-natanael/  
Portfolio: https://pedronatanaelfs.github.io/game.science/

---

## What I do
I build end-to-end data science projects that mirror how game studios work with data:
- Gameplay and balance analytics (match outcomes, skill signals, meta drivers)
- Product analytics (cohorts, retention, churn risk)
- Monetization analytics (segmentation, value/KPI movement)
- Experimentation (A/B testing, lift estimation, guardrails)
- Player voice (NLP on reviews, drivers of sentiment)
- Community analytics (viewer–creator dynamics, engagement signals)

---

## Featured portfolio projects (Game Data Science)

### 1) Gameplay Outcome Modeling — Early Game to Win Probability
<img width="768" height="229" alt="gameplay_outcome" src="https://github.com/user-attachments/assets/020c7ef1-ec07-436d-8b47-103d23b875a0" />

Goal: Predict match outcome using early-match signals and explain what drives wins.  
Skills: Feature engineering, classification, calibration, interpretability (SHAP), insight writing  

Dataset: League of Legends (Kaggle)  

Repo: (WIP)  
Deliverables: Model card, evaluation notebook, short insights report (PDF)

Why it matters:
- Balance & design decisions: Quantifying which early-game signals most reliably lead to wins helps designers identify mechanics that are too snowbally (or too irrelevant) and tune based on evidence, not vibes.
- Matchmaking quality: Outcome models help flag “unfair” matches (one-sided from minute 5) and support diagnostics for matchmaking issues, smurfing, or skill/rank inflation.
- Player coaching & in-game systems: Calibrated win-probability curves can power post-match insights, tutorials, and recommended focus areas, improving player experience.
- Live-ops monitoring: Sudden shifts in key drivers can signal patch impact and regressions early, before social channels blow up.
- Retention/business impact: Consistently unbalanced matches are a churn driver; modeling links match experience to retention proxies and helps prioritize fixes.
- Explainability turns a model into a tool: Studios won’t act on a black box. SHAP-style explainability converts predictions into actions teams can trust.


### 2) Retention and Churn Risk — Cohorts and Early Warning Scoring

<img width="768" height="229" alt="retention_and_churn" src="https://github.com/user-attachments/assets/f74dee7f-8960-41d5-86de-e7fd60bc819b" />

Goal: Build retention cohorts (D1/D7/D30), define churn, and score churn risk.  

Skills: Cohort analysis, retention curves, segmentation, model evaluation  

Dataset: Mobile analytics (Kaggle)  

Repo: (WIP)

Why it matters:
- Retention is the core health metric: For most games, especially live-service and F2P, retention drives everything downstream (revenue, matchmaking pool, community).
- Early warning enables intervention: If you can predict churn risk early, teams can trigger targeted actions (tutorial improvements, offers, push timing, content pacing).
- Better segmentation than “one-size-fits-all”: Cohorts and risk bands help tailor experiences for new users, returning users, and high-value players.
- Live-ops prioritization: The model helps identify which experiences correlate with drop-off (difficulty spikes, long sessions, paywalls, content gaps).
- Clear definitions reduce argument: A formal churn definition + metrics spec prevents teams from debating “what churn means” every time results look bad.

### 3) Experimentation — A/B Testing That Holds Up

<img width="768" height="229" alt="experimentation" src="https://github.com/user-attachments/assets/325b6ab6-fd0a-412d-992e-fa53afa70133" />

Goal: Evaluate experiment impact with confidence intervals, SRM checks, and guardrails.  

Skills: Hypothesis design, effect size estimation, slicing, variance reduction (optional)  

Dataset: Mobile analytics (Kaggle)  

Repo: (WIP)

Why it matters:
- It’s how games ship changes safely: Studios rely on experiments to change economy, onboarding, matchmaking, UI, and content without damaging the game.
- Guardrails prevent “winning” by breaking things: A change can lift revenue but harm retention, session quality, or fairness; guardrails keep decisions honest.
- Confidence intervals drive decisions, not vibes: Knowing the likely range of impact matters more than a single p-value.
- Detects data issues early: SRM checks and sanity tests catch pipeline or allocation problems before a bad decision goes live.
- Supports decision speed: A clean experimentation workflow reduces back-and-forth and helps teams ship improvements faster.

### 4) Player Voice (NLP) — What Players Complain About and Why It Matters

<img width="768" height="229" alt="player_voice_nlp" src="https://github.com/user-attachments/assets/7bbc32d8-0569-4db4-bdf8-3ed851df120e" />

Goal: Use topic modeling + sentiment analysis on reviews to identify the biggest drivers of negative feedback.  

Skills: NLP preprocessing, topic modeling/embeddings, interpretable modeling, trend analysis  

Dataset: Steam reviews (Kaggle)  

Repo: (WIP)

Why it matters:
- Reviews are a growth lever: Store ratings and review sentiment affect conversion and long-term discovery.
- Turns unstructured feedback into a roadmap: Topic clusters convert “a wall of text” into actionable themes (performance, bugs, balance, pricing).
- Measures impact of patches: Trend shifts by topic can show whether a fix actually reduced complaints or just moved them elsewhere.
- Detects reputational risks early: Spikes in specific complaint topics can be flagged before they become long-running negative narratives.
- Bridges teams: NLP summaries help product, engineering, and community teams align on what matters most.

### 5) Community Analytics — Twitch Interaction Graphs and Engagement

<img width="768" height="229" alt="community_analysis" src="https://github.com/user-attachments/assets/ed0b9481-a3ba-4bf1-81f7-19d5487b76ab" />

Goal: Model viewer–streamer interactions and build community health metrics and segments.  

Skills: Graph analytics, community detection, time-based features, forecasting (optional)  

Dataset: Twitch interactions (Kaggle)  

Repo: WIP

Why it matters:
- Community is part of the product: For many games, creator ecosystems and social engagement drive adoption and retention.
- Identifies healthy vs fragile communities: Graph structure can reveal whether engagement is broad-based or dependent on a few hubs.
- Supports creator programs: Segmentation can inform partnership targeting, drops campaigns, and incentives with measurable outcomes.
- Detects churn proxies: Returning viewers/chatters are a strong engagement signal, useful for forecasting and interventions.
- Helps allocate marketing spend: Data-backed attribution beats “we think this streamer is good for us.”

### 6) Live Ops Reporting — Monthly Game Health Dashboard

<img width="768" height="229" alt="live_ops" src="https://github.com/user-attachments/assets/619004a0-a450-4507-8602-1c5dc9b67060" />

Goal: Produce a monthly report with KPI definitions and a reproducible pipeline.  

Skills: Metrics design, data modeling, pipelines, BI-style reporting  

Data: Derived from the projects above  

Repo: (WIP)  

Deliverables: `metrics.md`, `report.pdf`, dashboard screenshots

Why it matters:
- Live-ops is operations, not vibes: Teams need consistent KPIs and a single source of truth to run a game week-to-week.
- KPI definitions prevent metric drift: `metrics.md` makes numbers reproducible and avoids “why doesn’t my DAU match yours?”
- Faster decisions: A recurring report surfaces issues early (retention dips, sentiment spikes, engagement drops) and shortens response time.
- Aligns stakeholders: One dashboard/report gives product, design, engineering, marketing, and leadership the same picture.
- Demonstrates production thinking: This shows you can ship analytics, not just notebooks.

---

## Toolbox
Python: pandas, numpy, scikit-learn, statsmodels  
NLP: spaCy, transformers (as needed), topic modeling  
Experimentation: hypothesis testing, confidence intervals, guardrails, SRM checks  
Data: SQL, data modeling, reproducible pipelines  
Visualization: notebooks and BI-style reports

---

## How I structure projects
Most repos include:
- README (problem → data → method → results → decision)
- `metrics.md` with KPI definitions
- `notebooks/` (EDA → modeling → insights)
- `src/` for reusable code
- a short `report.pdf`
- `requirements.txt` and reproducible runs

---

If you’d like to talk: pedronatanaelfs@gmail.com
