# AI-And-Automation-Projects
### 🧩 AI Requirements Assistant (Gemini Edition)
**Problem:** PMOs and BAs spend hours after every meeting manually turning raw notes into requirements, user stories, acceptance criteria, and risks.
**Solution:** A 4-stage AI pipeline (requirements → stories → acceptance criteria → risks) that generates a structured, ID-linked requirements package from raw meeting notes, powered by Google Gemini.
**Benefit:** Turns a multi-hour documentation task into a reviewable first draft in seconds, with a live traceability matrix and flagged ambiguities.

🔗 [Live demo](https://requirements-assistant.lovable.app)

### 🧩 AI Requirements Assistant (Claude Edition)
**Problem:** Same documentation bottleneck — plus the question of whether the same solution holds up across different AI platforms.
**Solution:** The identical 4-stage pipeline and traceability approach, built as a self-contained Claude Artifact calling the Claude API directly from the browser — no separate backend.
**Benefit:** The same working solution, shipped on two different AI platforms and architectures.

🔗 [Live demo](https://claude.ai/public/artifacts/12a7d036-bd35-435b-9b0a-c31a0750fc84) ·

### 🧩 AI-Assisted Expense Tracker (Claude Edition)
**Problem:** Translating business requirements directly into working software usually needs a traditional dev handoff, slowing delivery and diluting PM oversight along the way.
**Solution:** Built a full-stack expense tracking app end-to-end using Claude Code as an AI development partner, applying a "big prompt" methodology — describing complete feature requirements upfront rather than incremental prompting. Next.js, TypeScript, and Tailwind CSS, with expense data persisted client-side via localStorage. Explored three parallel implementation approaches (simple export, advanced multi-format export, cloud-integrated export) using Git branching to compare options before selecting a direction — mirroring real portfolio evaluation and delivery decisions.
**Benefit:** Shows the ability to direct AI-driven delivery end-to-end — requirements, build, quality review, and version control — while retaining PM-level oversight (reviewing every file change, approving every command) throughout, not just prompt engineering in isolation.

🔗 💻  [View code](https://github.com/San1203/expense-tracker-ai) · 

### 🧩 Custom Documentation Automation Command (Claude Edition)
**Problem:** Documentation debt — inconsistent, manually written, quickly-outdated docs — and the common failure of writing only for developers while end users are left without guidance.
**Solution:** Designed a reusable Claude Code slash command (/generate-docs) using a structured prompt-engineering framework (Task instructions, Arguments, Reusable process steps, Guided examples, Explicit outputs, Template naming, Error handling, Documentation). Given only a feature name, it analyzes the relevant code, classifies the feature as frontend/backend/full-stack, and generates two distinct, purpose-built documentation files: (1) a technical specification for developers — architecture, API details, and implementation notes — and (2) a user guide for non-technical readers — plain-language, step-by-step instructions with real captured screenshots. Both follow the project's existing documentation patterns, are cross-linked to each other, and are cross-referenced against related existing documentation.
**Benefit:** Demonstrates applying PMO governance instincts (standardization, dual-audience communication, traceability, built-in quality checks) directly to a technical AI workflow, rather than one-off AI usage.

🔗 💻  [View code](https://github.com/San1203/expense-tracker-ai/blob/master/.claude/commands/generate-docs.md) · 

### 🧩 Parallel Feature Development with Git Worktrees & AI Subagents (Claude Edition)
**Problem:** Serial AI development is slow when multiple independent features are ready to build at once — and parallel work risks silently hiding the coordination points that still need human judgment.
**Solution:** DDesigned and ran a parallel AI development workflow combining Git worktrees with Claude Code subagents — spinning up multiple isolated working directories, each on its own branch, and assigning an independent AI subagent to build a full feature in each simultaneously (no shared state, no interference). Used this to build two features in parallel and surfaced a genuine shared-dependency conflict during integration (both features independently modified the app's navigation component in incompatible ways), requiring a manual reconciliation decision.
**Benefit:** Demonstrates orchestration of multi-agent technical delivery and the PMO skill of identifying and resolving shared-dependency conflicts between concurrent workstreams — a direct technical analogue to managing parallel project tracks.
🔗 💻  [View code](https://github.com/San1203/expense-tracker-ai/branches) · 

### 📋 AI RAID & Status Digest *(Planned)*
**Problem:** Project status updates arrive scattered across emails, chats, and notes, making it hard to keep an accurate RAID log and executive status view current.
**Solution:** Converts scattered project updates into one consolidated executive status report with RAG status and a structured RAID log.
**Benefit:** Replaces a manual weekly compilation task with an automated, always-current status view for leadership.

### 📋 Vendor & SOW Governance Extractor *(Planned)*
**Problem:** Key vendor contract terms — renewal dates, obligations, risk clauses — are easy to lose track of across dozens of SOWs and contracts.
**Solution:** Extracts key terms, renewal dates, and risk flags directly from vendor contracts and SOWs.
**Benefit:** Reduces missed renewals and contract risk by surfacing critical terms automatically.

---

## Other Work

### 📊 Data Warehouse Solution
SQL-based data warehouse project with data modeling, ETL processes, and Power BI–connected reporting.

🔗 [Code](https://github.com/San1203/data-warehouse-solution)
