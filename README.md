# tlcp-study-guide
Free, open-source study guide for learning. This is meant to serve as an outline for those looking to keep track of their progress while they use the guided learning function LLMs have. Please feel free to fork it for your own use.

# ScholarOS: 50-Module Intensive Study Tracking Portal & Prompt Generator

A lightweight, zero-dependency, single-page application (SPA) designed for PhD preparation and high-register language mastery across 5 specialized academic tracks. Built with clean vanilla JavaScript and Tailwind CSS (CDN), requiring no build steps, Node.js, or backend servers.

---

## 🎯 Supported Curriculum Tracks (50 Pre-Seeded Modules)

1. **Track A: Calculus Foundations for Econometrics & Formal Modeling (`calc-01` to `calc-10`)**
   - Limits, continuity, power/product/quotient/chain rules
   - Exponential and logarithmic calculus, log-linearization, elasticities
   - Univariate optimization, concavity/convexity, second-derivative tests
   - Taylor series expansions and linear approximations (engine of the Delta Method)
   - Indefinite & definite integrals, substitution, integration by parts
   - Improper integrals, Leibniz's Rule, and continuous probability (PDFs, CDFs, moments)
   - Multivariate functions, partial derivatives, gradients, total differentials
   - Unconstrained multivariate optimization, Hessians, leading principal minors
   - Constrained optimization, Lagrangians, Kuhn-Tucker, Implicit Function & Envelope Theorems
   - Matrix calculus and quadratic forms ($\partial a'b / \partial b$, $\partial b'Ab / \partial b$) for OLS/GLS/GMM

2. **Track B: Applied Econometrics & Causal Inference (`econ-01` to `econ-10`)**
   - Matrix algebra of OLS, projection matrices ($P$ & $M$), Frisch-Waugh-Lovell
   - Gauss-Markov theorem, White HC & Liang-Zeger cluster-robust standard errors
   - Asymptotic theory: consistency, LLN, CLT, Continuous Mapping, and Delta Method
   - Endogeneity, omitted variable bias formulas, classical measurement error attenuation
   - Potential outcomes (Neyman-Rubin), DAGs, colliders, matching & IPW
   - Instrumental variables, 2SLS, weak instrument diagnostics, LATE, shift-share (Bartik)
   - Panel data: within-transformation (FE), RE, Hausman test, Mundlak, Nickell bias
   - Modern Difference-in-Differences, Goodman-Bacon decomposition, staggered TWFE pitfalls
   - Regression Discontinuity (Sharp & Fuzzy RDD) and Synthetic Control methods
   - Maximum Likelihood Estimation (Logit, Probit, count) and Spatial Econometrics (SAR, SEM)

3. **Track C: Political Economy, IPE & International Relations Theory (`pe-01` to `pe-10`)**
   - Collective action, public goods, Ostrom commons, and Political Coase Theorem
   - Social choice, Arrow's Impossibility, Median Voter Theorem, Veto Players, Selectorate Theory
   - Credible commitment, property rights, state capacity (North-Weingast, Acemoglu-Robinson, Tilly)
   - Redistribution, regime transitions, Varieties of Capitalism (Meltzer-Richard, Boix, Hall-Soskice)
   - Trade politics cleavages (Stolper-Samuelson, Ricardo-Viner, Melitz firm heterogeneity)
   - Open economy macroeconomics, Mundell-Fleming Trilemma, Frieden exchange rate politics
   - IR paradigms under anarchy: structural realism, neoliberal institutionalism, constructivism
   - Rationalist explanations for war and crisis bargaining (Fearon 1995, audience costs)
   - Two-Level Games (Putnam) and Open Economy Politics (OEP)
   - Economic statecraft, asymmetric vulnerability (Hirschman), and Weaponized Interdependence (Farrell-Newman)

4. **Track D: Professional & Academic Taiwanese Mandarin (`mandarin-01` to `mandarin-10`)**
   - Syntactic shift: converting spoken Chinese (口語) to formal written Chinese (書面語)
   - Nuanced causal connectives: 「緣於」、「鑑於」、「從而」、「致使」
   - Academic argumentation: rebuttals and counter-theses using formal discourse markers
   - Institutional & corporate governance lexicon (繁體中文: TWSE, MOPS, FSC standards)
   - Policy memorandum phrasing: administrative tone and calibrated epistemic hedging
   - Empirical methodology phrasing: describing data collection, panel models, endogeneity
   - Quantitative data narration: percentage points, inflection points, statistical significance
   - Cross-strait and East Asian geoeconomic discourse: de-risking, supply chain resilience
   - Formal epistolary correspondence: high-register communication with faculty and institutes
   - Academic oral delivery: conference slide transitions, introducing speakers, Q&A moderation

5. **Track E: Advanced Workplace & Academic Japanese (`jpn-01` to `jpn-10`)**
   - Keigo refinement: Kenjougo I (謙譲語I) vs. Kenjougo II / Teichougo (丁重語)
   - Academic symposium emceeing (司会進行・座長): openings, introductions, floor moderation
   - Research paper prose (論文調): formal academic register (「〜と考えられる」、「〜に起因する」)
   - Nuance disambiguation in Kango (漢語): 促進 vs. 推進, 懸念 vs. 憂慮, 検討 vs. 検証
   - Diplomatic refusals: cushion words (クッション言葉) and boundary setting
   - Parsing Japanese statutory disclosures (有価証券報告書, 決算短信)
   - Economic security & trade controls: 経済安全保障推進法, 外為法, dual-use technology
   - Scholarly critique delivery: asking rigorous questions without triggering face-threat
   - Slide presentation narration: pointing out anomalies, signaling causal mechanisms
   - Meeting facilitation: reconciling conflicting viewpoints and synthesizing consensus

---

## ⚡ Core Features

- **Standardized Gemini Prompt Generation**: 1-click modal assembling a 4-phase interactive learning prompt calibrated for Gemini's tutor mode (Diagnostic Triangulation $\rightarrow$ Calibrated Instruction $\rightarrow$ Active Application Drill $\rightarrow$ Session Mastery Ledger).
- **Comprehensive State Persistence**: Tracks status (`Not Started`, `In Progress`, `Mastered`, `Review Needed`), 1–5 mastery rating, and session notes/JSON ledgers automatically in browser `localStorage`.
- **Zero Lock-in Data Portability**: One-click **Export JSON** and **Import JSON** tools to back up and transfer your study ledger across devices.
- **Responsive Dark Mode UI**: Built with a sleek slate-900 / slate-800 aesthetic, color-coded per track, with quick-filter tabs, status dropdowns, and dynamic text search.

---

## 🚀 Deployment & Local Usage Guide

### Option 1: Run Locally (Instant)
1. Download or clone this repository.
2. Double-click `index.html` to open it in any modern browser (Chrome, Edge, Safari, Firefox).
3. No web server, dependencies, or terminal commands needed.

### Option 2: Deploy Free on GitHub Pages (Public Web URL)
Follow these exact steps to make your site accessible online:

1. **Verify File Placement**: Ensure `index.html` is located directly in the root directory of your repository (not inside a subfolder).
2. **Open Repository Settings**: Navigate to your GitHub repository and click on **Settings** (gear icon in the top navigation bar).
3. **Navigate to Pages**: In the left sidebar under the **Code and automation** section, click **Pages**.
4. **Configure Build and Deployment**:
   - Under **Source**, select **Deploy from a branch**.
   - Under **Branch**, select `main` (or `master`) from the branch dropdown.
   - In the folder dropdown right beside it, leave it as `/ (root)`.
   - Click **Save**.
5. **Wait for Deployment**:
   - Go to the **Actions** tab in your repository. You will see a workflow titled `pages build and deployment` running.
   - Once it shows a green checkmark (usually 30–60 seconds), return to **Settings** $\rightarrow$ **Pages**.
   - Your live URL will be displayed at the top: `https://<username>.github.io/<repository-name>/`.
6. **Launch & Study**: Open the link, select a module, click **Launch Prompt Engine**, copy the prompt, and paste it into Gemini.

---

## 🔒 Privacy & Data Handling
All progress, notes, and mastery scores remain 100% private and stored exclusively in your local browser's `localStorage`. No data is ever transmitted to an external server. Use **Export JSON** regularly to keep offline backups of your learning journey.
