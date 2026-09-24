# IT-Tools (live build)

Static production mirror of [CorentinTh/it-tools](https://github.com/CorentinTh/it-tools) —
"Collection of handy online tools for developers" — served via GitHub Pages.

- **Live:** https://coattails-droid.github.io/it-tools-live/
- **Upstream source:** `CorentinTh/it-tools`
- **Upstream commit built:** `d505845f918e946ec300af7b36efc107e2f66e9e` (2026-02-12)
- **Build command:** `BASE_URL=/it-tools-live/ pnpm build`
  (the repo's `vite.config.ts` reads the Vite base from the `BASE_URL` env var,
  falling back to `/`; the full npm script also runs `vue-tsc --noEmit` first)
- **Build date:** 2026-09-24
- **License:** GPL-3.0 (see `LICENSE` — verbatim copy of the upstream license)

Everything in this repo is the compiled static output of that build plus
`404.html` (a copy of `index.html`, so client-side routes keep working on
GitHub Pages) and `.nojekyll`. No source, no build tooling, no `node_modules`
is pushed here — rebuild from the upstream commit with the command above.

All tools run entirely client-side; nothing in the app needs a backend or
API keys, which is why it works as a pure static site.
