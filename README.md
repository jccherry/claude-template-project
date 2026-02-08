# Claude Code Template Project

A starter template for projects built with Claude Code. Includes structured documentation, CI configuration, and a `CLAUDE.md` with session instructions that ensure consistent, high-quality output.

## What's Included

- **`CLAUDE.md`** — Session instructions for Claude Code (branching, docs, testing, planning)
- **`docs/`** — Documentation templates: `FRONTEND.md`, `BACKEND.md`, `DATABASE.md`, `DEPLOYMENT.md`, `TESTS.md`
- **`.github/workflows/ci.yml`** — GitHub Actions CI scaffold
- **`.github/workflows/auto-tag.yml`** — Auto-creates semver tags on merge to `main`
- **`.gitignore`** — Reasonable defaults for common stacks

## Using This Template

### Option 1: GitHub Template (Recommended)

1. Click **"Use this template"** on the GitHub repo page.
2. Name your new repo and create it.
3. Clone your new repo and start building.

### Option 2: Clone and Reset Git History

```bash
# Clone the template
git clone https://github.com/jccherry/claude-template-project.git my-new-project
cd my-new-project

# Remove the template's git history
rm -rf .git

# Start fresh
git init
git add .
git commit -m "Initial commit from claude-template-project template"

# Point to your new remote
git remote add origin git@github.com:<your-user>/<your-repo>.git
git push -u origin main
```

### Option 3: Degit (No Git History)

```bash
npx degit jccherry/claude-template-project my-new-project
cd my-new-project
git init
git add .
git commit -m "Initial commit from claude-template-project template"
```

## After Cloning

1. Update this `README.md` with your project's summary, setup, and deployment instructions.
2. Fill in the `docs/` templates as your project takes shape.
3. Update `.github/workflows/ci.yml` with your actual build, lint, and test commands.
4. Update `CLAUDE.md` if your project has additional conventions.

## Documentation Structure

| File | Purpose |
|------|---------|
| `docs/FRONTEND.md` | Frontend architecture, dependencies, styling, state management |
| `docs/BACKEND.md` | Backend architecture, API design, auth, error handling |
| `docs/DATABASE.md` | Schema, migrations, indexes, backups |
| `docs/DEPLOYMENT.md` | Environment configs, deploy steps, rollback procedures |
| `docs/TESTS.md` | Test strategy, coverage targets, running tests |

## CI/CD

The included GitHub Actions workflow (`.github/workflows/ci.yml`) is a scaffold. Update it with your project's actual commands:

```yaml
# .github/workflows/ci.yml runs on every push and PR to main
# Edit the build, lint, and test steps to match your stack
```

## Auto Tagging

Every merge to `main` automatically creates a semver git tag via `.github/workflows/auto-tag.yml`.

**How it works:**
1. Add a label to your PR before merging: `semver:major`, `semver:minor`, or `semver:patch`
2. On merge, the workflow reads the label, bumps the version, and pushes a new tag
3. If no label is present, it defaults to a patch bump

Claude Code sessions are instructed (via `CLAUDE.md`) to assess the appropriate version bump and confirm with the user before labeling.

## README Template

When you start a new project from this template, your README should follow this structure:

```markdown
# Project Name

One-sentence description of what this project does.

## Quick Start

How to get running locally in <5 minutes.

## Development

Dev server, hot reload, environment setup.

## Deployment

### Dev
### Staging

## Architecture

Mermaid diagram or description of system components.
```
