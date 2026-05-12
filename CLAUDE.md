# Ridgeline Studio — Claude Context

## Studio

- **Name:** Ridgeline Studio
- **Operator:** Dalton (solo)
- **Location:** Saskatchewan, Canada
- **Model:** Boutique web agency upgrading local businesses into conversion-ready digital assets
- **Acquisition Target:** RoadHouse Capital

---

## Stack Standard

All client projects use the following stack unless otherwise noted in the client's `CLAUDE.md`:

- **Framework:** Next.js (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **Deployment:** Vercel
- **Package Manager:** npm (default)

---

## Repo Types

| Type | Description |
|---|---|
| `static-upgrade` | Brochure/informational site with no CMS |
| `cms-upgrade` | Content-managed site |
| `ecomm-upgrade` | E-commerce site |
| `lead-gen-upgrade` | Conversion-focused, contact forms, CTAs, lead capture |

---

## Repository Structure

- All client repos live under the **DollywoodDole** GitHub account
- Repos will be transferred to the RoadHouse Capital org upon acquisition
- This core repo (`Ridgeline-Studio-Core`) holds shared templates, docs, and the client registry

---

## Workflow

1. **GitHub first** — create the client repo on GitHub before touching local
2. **Clone** — `git clone` into the working directory
3. **Scaffold** — add `CLAUDE.md`, `CLIENT.md`, and `.env.example` from templates
4. **Vercel** — connect repo and deploy
5. **VSCode workspace** — open via `ridgeline.code-workspace`
6. **Claude Code session** — begin execution with full context loaded

---

## Active Clients

| Client | Repo | Type | Status |
|---|---|---|---|
| Bright Smiles Dental | `brightsmilesdental` | `lead-gen-upgrade` | Active |

---

## Relay Method

- **Strategy** is handled via [Claude.ai](https://claude.ai) (conversation, planning, architecture)
- **Execution** is handled via Claude Code (file writes, commits, scaffolding, builds)

---

## Notes

- Keep all code clean and handoff-ready at all times
- No unnecessary dependencies
- Each client repo must be self-contained and independently deployable
