# ironik.xyz

Website for ironik.xyz. It presents the timelike repos (`~/projects/timelike/`) and other projects.

## Constraints

- Plain static HTML. No build step, no framework, no generators.
- GitHub Pages serves `main` from the repo root, so `index.html` must stay at the root.
- Keep `CNAME` (the custom domain) and `.nojekyll` (turns Jekyll off). Never delete or rename them.
- Inline CSS only. Colors are tokens on `:root`, with a dark variant under `prefers-color-scheme: dark`.
  Reuse the existing tokens; don't add new hard-coded colors.
- The layout must work at phone width without horizontal scrolling.
- `.env` is excluded through `.git/info/exclude`. Never commit it or publish anything from it.

## Voice and copy

- Headline: **"Software explorers of the ungoverned future"**. It replaced an earlier, narrower line,
  "Tools for AI agents that work in a shell." Don't go back to describing ironik.xyz only as a
  maker of agent tooling.
- Under the headline is a poem, one line per line break. Keep the wording and lowercase exactly:

  > ironik stepping stones
  > raised above the water
  > wind plunges them clean in little waves
  > hopping muddies them again

- Don't rewrite, punctuate, or "improve" the poem.

## Project entries

- Take each project's description and status from that project's own source of truth, not from
  memory. For timelike, that's `~/projects/timelike/code/README.md` and
  `~/projects/timelike/bridge/governance-context.md`.
- Don't claim features the repo doesn't have yet. Mark status honestly, e.g. "in development".
- The timelike project is mentored (`plan/`, `code/`, `bridge/`). This site is not. Don't run
  mentor or SpecSwarm workflows here.
