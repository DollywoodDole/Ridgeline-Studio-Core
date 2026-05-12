# Client Onboarding SOP

Standard 6-step process for spinning up a new Ridgeline Studio client project.

---

## Step 1 — Create GitHub Repo

- Go to [github.com/DollywoodDole](https://github.com/DollywoodDole)
- Create a new **private** repository named after the client (e.g. `brightsmilesdental`)
- Initialize with a README
- Do not add a `.gitignore` or license at this stage — scaffold will handle it

---

## Step 2 — Clone Locally

```bash
git clone https://github.com/DollywoodDole/[repo-name].git
cd [repo-name]
```

---

## Step 3 — Scaffold

Copy and fill in the following files from `Ridgeline-Studio-Core/templates/`:

- `CLAUDE.md` — from `CLAUDE.md.template`
- `CLIENT.md` — from `CLIENT.md.template`
- `.env.example` — from `env.example.template`

Then scaffold the Next.js project:

```bash
npx create-next-app@latest . --typescript --tailwind --app --no-src-dir --import-alias "@/*"
```

Add the client to [clients/index.md](../clients/index.md) in this core repo.

---

## Step 4 — Vercel Deploy

- Go to [vercel.com](https://vercel.com) and import the GitHub repo
- Set framework to **Next.js**
- Add environment variables from `.env.example`
- Deploy

---

## Step 5 — VSCode Workspace

- Open `ridgeline.code-workspace` from `Ridgeline-Studio-Core/workspace/`
- Add the new client folder to the workspace if not already present
- Save the updated workspace file

---

## Step 6 — Claude Code Session

```bash
cd [repo-name]
claude
```

- Claude Code will load `CLAUDE.md` automatically
- Begin execution: layout, components, pages, integrations
- Strategy lives in Claude.ai; execution lives in Claude Code
