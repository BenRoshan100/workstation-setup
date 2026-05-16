# WORKSTATION_SETUP.md
# Ben's Claude Code Workstation — One-Time Setup Instruction

> Drop this file in any new project root and say:
> **"Read WORKSTATION_SETUP.md and build my full workstation structure."**
> Claude Code will create every file and folder listed below.
> After setup, delete this file and work from CLAUDE.md.

---

## INSTRUCTIONS FOR CLAUDE CODE

You are setting up a personal AI workstation for Ben Roshan D — a Data Scientist / Applied AI Engineer
based in Bangalore, India. This is a one-time setup. Create every file and folder below exactly as
specified. Do not skip any file. After creating all files, print a checklist confirming what was created.

---

## FILES AND FOLDERS TO CREATE

### 1. Root CLAUDE.md (project routing file)

Create file: `CLAUDE.md`

```markdown
# CLAUDE.md — Project Workstation
# Ben Roshan D | Data Scientist / Applied AI Engineer | Bangalore, India

## Who I am
- DS2 / Applied AI profile with 4+ years in fintech analytics
- Domain: UPI rewards, experimentation, LLM agents, fraud, lending
- Target: International MNC roles (Intuit, Adobe, Atlassian, Tide, Stripe)
- Exit window: Sep–Nov 2026 | Target CTC: ₹35–55 LPA

## Project overview
[FILL THIS IN PER PROJECT — replace this line with 2 sentences about what this project does]

## Architecture and specs
@docs/architecture.md
@docs/decisions.md
@docs/api-spec.md

## My rules and memory
@.claude/rules/memory-profile.md
@.claude/rules/memory-preferences.md
@.claude/rules/memory-decisions.md
@.claude/rules/memory-sessions.md
@.claude/rules/coding-standards.md

## Auto-Update Memory — MANDATORY

Update memory files AS YOU GO, not at the end of the session.

| Trigger | File to update |
|---------|---------------|
| New fact learned about me or my constraints | memory-profile.md |
| I state a preference about how things should work | memory-preferences.md |
| An architectural or technical decision is made | memory-decisions.md (with date) |
| A bug, workaround, or discovery is made | memory-sessions.md |
| A session ends with something shipped or learned | memory-sessions.md |

**DO NOT ASK PERMISSION. Just update the file when the trigger fires.**
**DO NOT wait until the end of the session. Update immediately.**

## Operating modes

When I say **"Start session"** → run a structured 60–90 min session: concept → drill → build → reflect
When I say **"Build mode"** → work step by step on the current project
When I say **"Mock interview"** → switch to interviewer mode using my real projects
When I say **"Career audit"** → evaluate my market readiness using memory files
When I say **"Portfolio review"** → assess case study quality vs global DS standards

## Output style
- Direct, structured, high-density. No fluff.
- Tables for comparisons. Checklists for execution. Code blocks for everything runnable.
- Quantify in INR where relevant.
- Always connect: skill → project → impact → resume bullet → interview story.
```

---

### 2. Memory: Profile

Create file: `.claude/rules/memory-profile.md`

```markdown
# memory-profile.md
# Facts about Ben — updated as Claude learns new things

## Identity
- Full name: Ben Roshan D
- Location: Bangalore, India (IST, UTC+5:30)
- Current role: Data Scientist 2, Kotak 811
- Current CTC: ₹25 LPA | Take-home: ~₹1.68L/month
- Total experience: 4+ years in fintech analytics

## Career history (brief)
- Kotak 811: DS2 — UPI rewards analytics, LLM agent on AWS Bedrock (Jul 2025–present)
- Jupiter Money: DA2 — loan funnel, risk, cross-sell (Dec 2024–Jul 2025)
- Namma Yatri: DA2 — ride growth, surge pricing, driver retention (Feb 2023–Dec 2024)
- Coda Payments: Sr DA — fraud analytics, 65+ countries (Dec 2021–Feb 2023)
- Genpact: Sr Associate AML — transaction monitoring (Jan 2021–Nov 2021)

## Key shipped work (for interview stories)
- AWS Bedrock AI agent: reduced experiment analysis TAT from 3 days → 15 mins
- UPI value share uplift: 12.5% → 19% via AMB-tiered reward experiments
- Jupiter PF cap recommendation: prevented 22% → 10% conversion crash in premium segment
- Jupiter TPAP cross-sell: 45% approval rate vs 8% control → ₹2Cr/month new loan opportunity
- Namma Yatri surge engine: city-wide dynamic pricing across 8 Bangalore geohashes
- Namma Yatri cancellation reduction: 20% → 14% via micro-funnel optimization

## Constraints
- 90-day notice period at Kotak 811
- Career growth time: 60–90 minutes/day (morning 30 min + evening 60 min)
- Financial runway: ~₹16K/month surplus — razor thin, no buffer for income gap

## Exit target
- Companies: Intuit, Adobe, Atlassian, Tide, SAP, Microsoft/LinkedIn (primary)
- Stretch: Stripe, Wise, Monzo, Revolut, Brex, Plaid
- Floor CTC: ₹35 LPA from any international MNC
- Exit window: September–November 2026

## Education
- MBA Business Analytics, CMS Business School Jain University — CGPA 8.91
- BE Electrical & Electronics, Kumaraguru College of Technology — CGPA 8.37

## Online presence
- Blog: museeduben.art.blog
- GitHub: Ben Roshan
- LinkedIn: Ben Roshan

## [ADD FACTS HERE AS CLAUDE LEARNS THEM]
```

---

### 3. Memory: Preferences

Create file: `.claude/rules/memory-preferences.md`

```markdown
# memory-preferences.md
# How Ben likes things done — update when preferences are stated

## Code preferences
- Default language: Python
- Preferred ML stack: XGBoost, scikit-learn, SHAP, FastAPI, Streamlit
- Preferred GenAI stack: Claude API, LangChain, LangGraph, ChromaDB, MCP SDK
- Preferred cloud: AWS (Bedrock, Redshift, Athena) — but deploy portfolio to Railway or Render
- Preferred DB: SQLite for local dev, Redshift/Postgres for prod
- Preferred BI: PowerBI at work, Metabase for internal tools

## Output preferences
- No long preambles. Get to the answer.
- Tables over bullet lists for comparisons
- Checklists for execution steps
- Always include time estimates for tasks
- Quantify in INR, not USD, unless role is international remote
- Connect everything: concept → code → impact → resume bullet

## Learning preferences
- Build something in 30 mins for every new concept learned — no passive note-taking
- Prefer action-oriented sessions: concept (10 min) → drill (20 min) → build (40 min) → reflect (10 min)
- Use real fintech problems as examples, not generic toy problems

## Project preferences
- Every project ships with: GitHub README + live demo URL + LinkedIn post
- README structure: problem → architecture → demo GIF → results table → how to run locally
- LinkedIn post on ship day: 200 words max, link to demo

## Communication preferences
- Be direct about gaps and inefficiencies — no cushioning unless asked
- Call out stagnation if sessions produce no shipped output
- If two options exist, recommend the higher-leverage one, not the easier one

## [ADD PREFERENCES HERE AS THEY ARE STATED]
```

---

### 4. Memory: Decisions

Create file: `.claude/rules/memory-decisions.md`

```markdown
# memory-decisions.md
# Technical and architectural decisions — add with date when made

## Format for new entries
### [YYYY-MM-DD] — [Project] — [Decision title]
- **Decision:** What was decided
- **Rationale:** Why
- **Trade-off:** What was given up
- **Status:** Active / Superseded

---

## Existing decisions

### [2026-05] — Global — Deployment platform
- **Decision:** Use Railway for portfolio project deployments (not Render)
- **Rationale:** Railway has better cold-start behaviour and simpler env var management
- **Trade-off:** Slightly less free tier headroom than Render
- **Status:** Active

### [2026-05] — Global — Claude Code memory architecture
- **Decision:** Split memory into 4 files under .claude/rules/ (profile, preferences, decisions, sessions)
- **Rationale:** Keeps CLAUDE.md under 200 lines; each file is auto-loaded and independently updatable
- **Trade-off:** More files to manage vs single CLAUDE.md knowledge dump
- **Status:** Active

### [2026-05] — Global — Portfolio stack
- **Decision:** VerdictAI (existing) → PropensityAPI → FinRAG → DataMCP → UnderwriteAI → MemoryOS
- **Rationale:** Covers all GenAI topics systematically; each project covers distinct skill gap
- **Trade-off:** Long roadmap; first 2 projects must ship before applications go live
- **Status:** Active

## [ADD NEW DECISIONS HERE WITH DATE AND PROJECT]
```

---

### 5. Memory: Sessions

Create file: `.claude/rules/memory-sessions.md`

```markdown
# memory-sessions.md
# Rolling session log — append after each substantive session

## Format for new entries
### [YYYY-MM-DD] — [Project] — [What happened]
- **Shipped:** What was completed
- **Discovered:** Non-obvious learning, bug, or workaround
- **Blockers:** What's stuck and why
- **Next:** Immediate next action

---

## [SESSION LOG STARTS HERE — Claude appends as sessions complete]
```

---

### 6. Coding Standards

Create file: `.claude/rules/coding-standards.md`

```markdown
# coding-standards.md
# Ben's coding standards for all portfolio projects

## Python
- Use Python 3.11+
- Format with black (line length 88)
- Type hints on all function signatures
- Docstrings on all public functions (one-line for simple, full for complex)
- requirements.txt for every project — pin major versions

## FastAPI
- Router-based structure (not monolithic main.py)
- Pydantic models for all request/response schemas
- /health endpoint on every API
- Log all requests with timing

## ML projects
- Separate notebooks/EDA/ from src/ — notebooks are exploration, src/ is production
- Always include a baseline model before the real model
- Evaluation: always show Precision@K, Recall@K, AUC alongside accuracy
- SHAP explanations mandatory for any production-bound classifier

## GenAI / LLM projects
- Separate prompt templates into prompts/ directory
- Log all LLM calls with input/output/latency/tokens
- Evaluation metrics defined before building (faithfulness, relevance, etc.)
- Never hardcode API keys — always use .env + python-dotenv

## Git
- Branch: feature/[short-name] or fix/[short-name]
- Commits: conventional commits style (feat:, fix:, docs:, refactor:)
- Every project has a .gitignore that excludes .env, __pycache__, *.pyc, .DS_Store

## README structure (mandatory for every project)
1. Problem statement (2-3 sentences)
2. Architecture diagram or description
3. Demo GIF or screenshot
4. Results table (metrics vs baseline)
5. How to run locally (copy-paste commands)
6. Tech stack badges
```

---

### 7. Architecture doc (template)

Create file: `docs/architecture.md`

```markdown
# Architecture — [Project Name]

## Problem
[2 sentences: what problem does this solve, who is the user]

## Architecture overview
[Describe the system: data flow, components, APIs, databases]

## Component breakdown

| Component | Technology | Purpose |
|-----------|------------|---------|
| [name] | [tech] | [what it does] |

## Data flow
1. [Step 1]
2. [Step 2]
3. [Step 3]

## Key design decisions
- [Decision 1 and why]
- [Decision 2 and why]

## Known limitations
- [Limitation 1]

## Future improvements
- [Improvement 1]
```

---

### 8. Decisions doc (template)

Create file: `docs/decisions.md`

```markdown
# Technical Decisions — [Project Name]

## Decision log

| Date | Decision | Rationale | Status |
|------|----------|-----------|--------|
| [date] | [what] | [why] | Active |

## Rejected alternatives
[Document things you considered but didn't use, and why — this is useful for interviews]
```

---

### 9. API spec (template)

Create file: `docs/api-spec.md`

```markdown
# API Specification — [Project Name]

## Base URL
`https://[your-project].railway.app`

## Endpoints

### POST /score
**Purpose:** [describe]
**Request:**
```json
{
  "field": "type"
}
```
**Response:**
```json
{
  "result": "type"
}
```
**Example curl:**
```bash
curl -X POST https://[url]/score \
  -H "Content-Type: application/json" \
  -d '{"field": "value"}'
```

### GET /health
**Purpose:** Health check
**Response:** `{"status": "ok", "version": "1.0.0"}`
```

---

### 10. Hook: Stop hook script

Create file: `.claude/hooks/session-reflect.sh`

```bash
#!/bin/bash
# Stop hook — fires when Claude finishes a session
# Checks for learning signals and reminds Claude to update memory files

CONTEXT=$(cat)

# Strong signals — definitely learned something
STRONG_PATTERNS="fixed|workaround|gotcha|that's wrong|check again|we already|should have|discovered|realized|turns out|doesn't work|found out|the issue was|root cause"

# Weak signals — might have learned something
WEAK_PATTERNS="error|bug|issue|problem|fail|unexpected|surprising|odd"

if echo "$CONTEXT" | grep -qiE "$STRONG_PATTERNS"; then
    cat << 'EOF'
{
  "decision": "approve",
  "systemMessage": "MEMORY UPDATE REQUIRED: This session involved fixes, discoveries, or workarounds. Before closing: (1) Add entry to memory-sessions.md with what was discovered. (2) If an architectural decision was made, add to memory-decisions.md with today's date. (3) If you learned something new about Ben's preferences, update memory-preferences.md. Do this now."
}
EOF
elif echo "$CONTEXT" | grep -qiE "$WEAK_PATTERNS"; then
    cat << 'EOF'
{
  "decision": "approve",
  "systemMessage": "This session may have involved learning. If anything non-obvious was discovered, run /reflect or manually update memory-sessions.md before closing."
}
EOF
else
    echo '{"decision": "approve"}'
fi
```

---

### 11. Hook settings

Create file: `.claude/settings.json`

```json
{
  "hooks": {
    "Stop": [
      {
        "matcher": "",
        "hooks": [
          {
            "type": "command",
            "command": "bash .claude/hooks/session-reflect.sh"
          }
        ]
      }
    ]
  }
}
```

---

### 12. Project README (template)

Create file: `README.md`

```markdown
# [Project Name]

> [One sentence: what it does and why it matters]

![demo](docs/demo.gif)

## Problem
[2-3 sentences: what problem this solves, who has this problem]

## Architecture
[Description or diagram of how the system works]

## Results

| Metric | Baseline | This model |
|--------|----------|-----------|
| [metric] | [value] | [value] |

## Tech stack
- **ML:** [libraries]
- **API:** FastAPI
- **Frontend:** Streamlit
- **Deploy:** Railway

## Run locally
```bash
git clone [repo-url]
cd [project]
pip install -r requirements.txt
cp .env.example .env  # add your API keys
uvicorn main:app --reload
```

## Case study
[Link to blog post on museeduben.art.blog]

## Portfolio context
This project is part of my Data Science / Applied AI portfolio targeting international MNC roles.
Built to demonstrate: [specific skill 1], [specific skill 2], [specific skill 3].
```

---

### 13. Environment template

Create file: `.env.example`

```
# Copy this to .env and fill in your values
# Never commit .env to git

ANTHROPIC_API_KEY=your_key_here
DATABASE_URL=sqlite:///./data/app.db
ENVIRONMENT=development
LOG_LEVEL=INFO
```

---

### 14. Gitignore

Create file: `.gitignore`

```
# Environment
.env
.env.local

# Python
__pycache__/
*.py[cod]
*.pyo
*.pyd
.Python
*.egg-info/
dist/
build/
.eggs/
venv/
.venv/
env/

# Notebooks (keep .ipynb, ignore checkpoints)
.ipynb_checkpoints/

# Data (keep structure, ignore raw data files)
data/raw/*.csv
data/raw/*.parquet
data/raw/*.json
*.pkl
*.joblib

# OS
.DS_Store
Thumbs.db

# IDE
.vscode/
.idea/
*.swp

# Claude local settings (personal, not shared)
.claude/settings.local.json

# Models (too large for git)
models/*.pkl
models/*.joblib
models/*.bin
```

---

### 15. Project structure readme

Create file: `docs/structure.md`

```markdown
# Project Structure

```
project/
├── CLAUDE.md                    ← Claude Code routing file (read every session)
├── README.md                    ← Public-facing project readme
├── requirements.txt             ← Python dependencies
├── .env.example                 ← Environment variable template
├── .gitignore
│
├── .claude/
│   ├── settings.json            ← Hook configuration
│   ├── hooks/
│   │   └── session-reflect.sh  ← Stop hook for memory updates
│   └── rules/
│       ├── memory-profile.md    ← Facts about Ben (auto-updated)
│       ├── memory-preferences.md← How Ben likes things done (auto-updated)
│       ├── memory-decisions.md  ← Technical decisions with dates (auto-updated)
│       ├── memory-sessions.md   ← Session log (auto-updated)
│       └── coding-standards.md ← Code style rules
│
├── docs/
│   ├── architecture.md          ← System design
│   ├── decisions.md             ← Project-level decisions
│   ├── api-spec.md              ← API documentation
│   └── structure.md             ← This file
│
├── src/                         ← Production code
│   ├── __init__.py
│   ├── main.py                  ← FastAPI app entry point
│   ├── models/                  ← ML model code
│   ├── api/                     ← API routes
│   ├── utils/                   ← Shared utilities
│   └── prompts/                 ← LLM prompt templates
│
├── notebooks/
│   └── EDA/                     ← Exploratory notebooks (not production)
│
├── data/
│   ├── raw/                     ← Source data (gitignored if large)
│   └── processed/               ← Cleaned, feature-engineered data
│
├── tests/
│   └── test_api.py
│
└── models/                      ← Saved model artifacts (gitignored)
```
```

---

## VERIFICATION CHECKLIST FOR CLAUDE CODE

After creating all files, confirm the following exist:

```
[ ] CLAUDE.md
[ ] README.md
[ ] .env.example
[ ] .gitignore
[ ] .claude/settings.json
[ ] .claude/hooks/session-reflect.sh
[ ] .claude/rules/memory-profile.md
[ ] .claude/rules/memory-preferences.md
[ ] .claude/rules/memory-decisions.md
[ ] .claude/rules/memory-sessions.md
[ ] .claude/rules/coding-standards.md
[ ] docs/architecture.md
[ ] docs/decisions.md
[ ] docs/api-spec.md
[ ] docs/structure.md
```

Also run:
```bash
chmod +x .claude/hooks/session-reflect.sh
```

Then confirm: "Workstation setup complete. All 15 files created. Hook is executable.
Fill in the [Project overview] section of CLAUDE.md and you're ready to build."

---

## HOW TO USE THIS FOR EVERY NEW PROJECT

1. Copy this file into the new project folder
2. Open Claude Code in that folder
3. Say: **"Read WORKSTATION_SETUP.md and build my full workstation structure."**
4. Wait for Claude to create all files and confirm the checklist
5. Edit `CLAUDE.md` — replace the `[FILL THIS IN PER PROJECT]` line with 2 sentences about the new project
6. Delete `WORKSTATION_SETUP.md`
7. Start building

**That's it. The memory system is live from session one.**