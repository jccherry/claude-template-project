# Claude Code Project Instructions

These instructions are mandatory for all Claude Code sessions working in this repository.

## Session Startup

1. **Read all docs first.** Before writing any code, read every file in `docs/` to understand the current state of the project — architecture, conventions, deployment, and test strategy.
2. **Work on a clean branch.** Always create a new branch off `main` for any feature, improvement, or bugfix. Use conventional branch names: `feat/`, `fix/`, `refactor/`, `docs/`, `chore/`.
3. **Understand before acting.** Review relevant source files before making changes. Never modify code you haven't read.

## Planning & Requirements

Before starting implementation, ask probing questions to:

- **Clarify requirements** — What exactly should this do? What inputs/outputs are expected?
- **Identify hard requirements** — What constraints are non-negotiable (performance, compatibility, security)?
- **Identify soft requirements** — What's preferred but flexible (naming, UI layout, specific libraries)?
- **Discover hidden requirements** — What edge cases, error states, or integrations haven't been mentioned?
- **Confirm scope** — What's explicitly out of scope for this change?

Do not assume. When in doubt, ask.

## Code Style

- **Be concise and modern.** Use current language features and idiomatic patterns.
- **Comments: reasonable, not verbose.** Comment the "why", not the "what". Skip obvious comments. Add comments for non-obvious logic, workarounds, and business rules.
- **No over-engineering.** Solve the problem at hand. Don't build abstractions for hypothetical future needs.

## Testing

- **Always include tests.** Every feature or bugfix should have corresponding tests.
- **Keep CI green.** Ensure GitHub Actions CI passes before requesting review.
- **Test edge cases.** Cover error paths and boundary conditions, not just the happy path.

## Documentation

- **Keep `docs/` up to date.** When you change code, update the relevant doc files in the same commit.
- **Co-locate doc changes with code changes.** Don't make a separate commit for docs — include them with the code they describe.
- **Update `README.md`** if your change affects setup, deployment, or architecture.

## Git Workflow

- Branch off `main` for all work.
- Write clear, descriptive commit messages summarizing the "why".
- Keep commits atomic — one logical change per commit.
- Include doc updates in the same commit as the related code change.

## CI/CD

- All projects must include GitHub Actions CI that runs linting and tests.
- CI must pass before merging to `main`.
- Keep CI configuration in `.github/workflows/`.

## README Standards

Every project README should include:

1. **Top-level summary** — What the project does, in 1-2 sentences.
2. **Quick start** — How to get running locally.
3. **Dev deployment** — How to deploy to a dev environment.
4. **Staging deployment** — How to deploy to staging.
5. **Architecture diagram** — If the system has multiple components, include a diagram (Mermaid preferred).
