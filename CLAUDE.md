# Project instructions for Claude Code

## About this project
<!-- One or two sentences: what this repo is, primary language/framework, how to run it. -->

## Working preferences

### Pull requests
- Create PRs as **ready for review**, not as draft.
- Keep PR titles under 70 characters; put detail in the body.
- Include a short "Summary" and "Test plan" section.

### Commits
- Write concise commit messages focused on *why*, not *what*.
- Create new commits rather than amending, unless explicitly asked.
- Never use `--no-verify` or skip hooks.

### Code style
- Prefer editing existing files over creating new ones.
- Don't add comments that just restate the code.
- Don't add speculative abstractions, error handling, or backwards-compat shims for scenarios that can't happen.
- Match the existing patterns in the file you're editing.

### Scope discipline
- Do only what was asked. No drive-by refactors, no new features, no "while I'm here" cleanup.
- If you notice something worth fixing, mention it — don't silently change it.

## Commands
<!-- Fill these in per-project -->
- Install: `...`
- Test: `...`
- Lint / typecheck: `...`
- Dev server: `...`

## Gotchas
<!-- Anything non-obvious: unusual build steps, framework quirks, files not to touch, etc. -->

