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

- Headline: **"Software explorers of the ungoverned future"**, with a line break after
  "explorers". It replaced an earlier, narrower line,
  "Tools for AI agents that work in a shell." Don't go back to describing ironik.xyz only as a
  maker of agent tooling.
- Under the headline is a poem, one line per line break. Keep the wording and lowercase exactly:

  > ironik stepping stones
  > raised above the water
  > wind plunges them clean in little waves
  > hopping muddies them again

- Don't rewrite, punctuate, or "improve" the poem.
- The poem is overlaid in white on the left of a full-column-width stepping-stones photo, over a
  semi-transparent dark shade (`--on-photo` and `--shade` tokens, the same in both themes). The poem is
  top-aligned with line-height 3.2, and its top padding matches the gap between lines. The photo
  is `stepping-stones.jpg`, a 1280px web copy of `1359407958_9c1cf76fb3_k.jpg`, which stays out of
  git. Its attribution sits right-aligned below it and must stay: "Bodies in Motion by Paul
  Stevenson", linking to https://www.flickr.com/photos/pss/1359407958/.
- The favicon (`favicon.ico`, plus `apple-touch-icon.png`) is the "K" cropped square out of the
  hakubun stamp, red background and all.
- The hakubun seal (`hakubun.png`) sits at the bottom of the footer, aligned left, linking to
  https://ironik.xyz. It's a cropped, transparent web copy of the original artwork
  `Hakubun 2 — archaic, heavy.png`, which stays out of git.

## Project entries

- Take each project's description and status from that project's own source of truth, not from
  memory. For timelike, that's `~/projects/timelike/code/README.md` and
  `~/projects/timelike/bridge/governance-context.md`.
- Don't claim features the repo doesn't have yet. Mark status honestly, e.g. "in development".
- The timelike project is mentored (`plan/`, `code/`, `bridge/`). This site is not. Don't run
  mentor or SpecSwarm workflows here.
