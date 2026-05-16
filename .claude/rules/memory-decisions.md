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
