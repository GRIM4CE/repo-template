# Project instructions for Claude Code

## About this project
<!-- One or two sentences: what this repo is, primary language/framework, how to run it. -->

## Working preferences

### Pull requests
- Create PRs as **ready for review**, not as draft.
- Keep PR titles under 70 characters; put detail in the body.
- Include a short "Summary" and "Test plan" section.
- Keep PRs small and focused on a single concern. If a change is growing large, split it into a stack of smaller, independently reviewable PRs.

### Commits
- Write concise commit messages focused on *why*, not *what*.
- Create new commits rather than amending, unless explicitly asked.
- Never use `--no-verify` or skip hooks.
- Keep commits atomic (one logical change per commit).

### Git
- Don't force push.
- Don't modify git config or hooks.

### Code style
- Prefer editing existing files over creating new ones.
- Don't add comments that just restate the code.
- Don't add speculative abstractions, error handling, or backwards-compat shims for scenarios that can't happen.
- Match the existing patterns in the file you're editing.

### Code structure
- Stay DRY, but follow the rule of three: don't abstract on the first duplicate. Wrong abstractions are costlier than repetition.
- Keep new files focused on one responsibility. If a file you're already editing has drifted into multiple concerns, flag it rather than splitting it mid-task.
- Build UI with a design-system mindset: presentational components stay dumb (props in, markup out), and business logic lives in hooks, services, or containers. Apply the same rule-of-three trigger for extracting shared components — consolidate once a pattern repeats, not before.

### Scope discipline
- Do only what was asked. No drive-by refactors, no new features, no "while I'm here" cleanup.
- If you notice something worth fixing, mention it — don't silently change it.

### Dependencies
- Prefer LTS or current stable releases for languages and runtimes; only move off LTS when a specific feature or fix requires it, and note why in the PR.
- Pin or constrain versions in line with the ecosystem's conventions (lockfiles, version ranges).
- Dependabot is enabled by default (see `.github/dependabot.yml`); keep minor/patch updates grouped to limit PR noise.

### Safety
- Never commit secrets, API keys, or credentials.
- Don't delete or overwrite files without reading them first.
- Ask before making destructive changes (dropping tables, force pushing, etc.).

### Communication
- If something is unclear, ask rather than guess.
- If you notice unrelated issues, mention them but don't fix them.
- Be direct about trade-offs or concerns.

## Commands
<!-- Fill these in per-project -->
- Install: `<package-manager> install`
- Test: `<test-command>`
- Lint / typecheck: `<lint-command>`
- Dev server: `<dev-command>`

## Gotchas
<!-- Anything non-obvious: unusual build steps, framework quirks, files not to touch, etc. -->

