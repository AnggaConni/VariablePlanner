# 🧠 Variable Planner

> **An interactive, bilingual research framework visualizer** — map variables, model relationships, and get AI-powered analysis for academic research, behavioral science, and systems thinking.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Open%20App-6366f1?style=for-the-badge&logo=googlechrome&logoColor=white)](YOUR_DEMO_URL_HERE)
[![License: AGPL v3](https://img.shields.io/badge/License-AGPLv3-10b981?style=for-the-badge)](LICENSE)
[![Language](https://img.shields.io/badge/Language-EN%20%2F%20ID-f59e0b?style=for-the-badge)](README.md)

---

## ✨ What It Does

Variable Planner is a single-page, no-install tool for building and analyzing research frameworks. It's built for:
- **Thesis & dissertation students** mapping independent, dependent, mediating, and moderating variables
- **Researchers** modeling causal logic, DAGs, or SEM structures
- **Program designers** building Theory of Change (ToC) or COM-B behavioral models
- **Anyone** who needs to diagram cause-and-effect relationships visually

---

## 🖼️ Key Features

### 📋 Data Input Mode
Manage your variables and relationships in a clean form-based panel.
- Add variables with names, types, and research notes
- Define directional relationships between any two variables
- Auto-generate hypothesis labels (H1, H2, H3…)

### 🎨 Visual Mode — Two Layouts

| **Freeform Canvas** | **Framework View** |
|---|---|
| Drag-and-drop nodes freely | Auto-arranged into 4 semantic columns |
| Click "Connect" to draw edges | Animated glowing particle flow along edges |
| Pan, zoom, and auto-arrange | Neon cyber aesthetic, perfect for presentations |

### 🔬 40+ Variable Type Dictionary

Variables are categorized into three groups:

**Basic** — `Independent (X)`, `Dependent (Y)`, `Intervening`, `Moderator`, `Confounding`, `Outcome`, `Treatment`, `Baseline`, and more

**Advanced** — `Latent`, `Manifest`, `Mediator`, `Collider`, `Exogenous`, `Endogenous`, `Instrumental (IV)`, `Interaction Term`, `Lagged`, and more

**Statistical** — `Predictor`, `Criterion`, `Nominal`, `Ordinal`, `Interval`, `Ratio`, `Binary`, `Dummy`, `Continuous`, `Discrete`, and more

**Theory of Change** — `Input`, `Activity`, `Direct Output`, `Long-term Impact`

**COM-B Behavioral** — `Capability`, `Opportunity`, `Motivation`, `Target Behavior`

### 🔗 5 Relationship / Edge Types

| Type | Symbol | Color | Use case |
|---|---|---|---|
| Neutral | — | Gray | General flow, foundational links |
| Positive | + | Green | Amplifying / reinforcing effects |
| Negative | − | Rose | Dampening / destructive effects |
| Hypothesis | H | Indigo | Testable research propositions (H1, H2…) |
| Bidirectional | ↔ | Amber | Mutual causation, feedback loops |

---

## 🤖 AI Analysis (Gemini — Bring Your Own Key)

Powered by **Google Gemini 2.5 Flash**. Your API key stays in your browser's `localStorage` — it is never sent to any server other than Google's API directly.

### Framework Analyzer
Click the robot icon (🤖) in the top bar to analyze your entire framework:
- **Analysis tab** — Narrative evaluation of your model's logic and theoretical grounding
- **Mapping tab** — Topology health checks: detects floating nodes, bottlenecks, missing paths, and structural redundancies
- **Recommendations tab** — Suggests new variables to add, with types and rationale. Accept to add them to the canvas in one click. Ask AI to revise with custom instructions.

### Per-Node Deep Research
Select any variable, open the sidebar Edit tab, and click **"Deep AI Research Report"**:
- **Resume & Analysis** — Theoretical definition, measurement metrics, potential bias sources
- **Expansion** — Suggested predictor variables (causes) and outcome variables (effects), each addable to canvas with one click
- **Literature & Media** — Auto-linked Google Scholar paper, PubMed paper, and an embedded YouTube search result. All AI-generated and ready to explore.

---

## 📦 Sample Datasets

Load any of these from the **File / Records** menu:

| Sample | Description |
|---|---|
| **Thesis Framework** | Full academic SEM model — antecedent → X1, X2 → mediators → Y, with dummy controls and hypothesis edges |
| **Romance Scenario** | A playful causal logic map: "How to get your ex back" — uses intervening, moderator, and confounding variables |
| **Theory of Change** | Input → Activity → Output → Impact model with exogenous factors |
| **COM-B Model** | Behavioral diagnosis framework: Capability + Opportunity + Motivation → Behavior |

---

## 💾 Save & Export

- **Save JSON** — Exports your full canvas (nodes, edges, AI analysis data) as a `.json` file for later loading
- **Load JSON** — Reload any previously saved session
- **Export PNG** — Auto-centers and fits all nodes into frame, then captures a high-resolution `2×` PNG. Works in both Canvas and Framework view.

---

## 🌐 Bilingual Support

The entire interface — labels, dictionaries, variable type names, placeholder text, and AI prompt instructions — supports both **English** and **Indonesian (Bahasa Indonesia)**. Toggle with the `EN / ID` button in the navbar. AI analysis results will also be returned in your active language.

---

## 🚀 Getting Started

No build step, no dependencies, no server required. It's a single HTML file.

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/variable-planner.git

# Open in browser — that's it
open index.html
```

Or just open the [live app (beta)]([https://anggaconni.github.io/VariablePlanner/]) directly.

### For AI features
1. Get a free Gemini API key from [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Click the 🤖 robot icon in the top bar
3. Paste your key (format: `AIzaSy...`) and click **Start Analysis**

---

## 🧱 Tech Stack

| Layer | Tech |
|---|---|
| UI Framework | React 18 (CDN, via Babel standalone) |
| Styling | Tailwind CSS (CDN) |
| Markdown rendering | `marked.js` |
| PNG export | `html2canvas` |
| AI | Google Gemini 2.5 Flash API |
| Fonts | Plus Jakarta Sans, JetBrains Mono, Material Symbols Rounded |

No build tool. No npm install. Everything loads from CDN — the entire app is one `index.html` file.

---

## 📁 Project Structure

```
variable-planner/
└── index.html       # The entire application — all JS, CSS, and markup in one file
```

---

## 🗺️ Roadmap Ideas

- [ ] Collaborative editing (multi-user canvas)
- [ ] Mermaid / DOT export
- [ ] Custom variable type creator
- [ ] Hypothesis auto-numbering across sessions
- [ ] PDF export with dictionary appendix

---

## 📄 License

AGPL — free to use, fork, and modify.
