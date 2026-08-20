# test-visual-novel-1

A generated visual novel — the example project used to exercise VN Generator's web export.

**Read it here:** https://joeedh.github.io/test-visual-novel-1/

Every push to `master` runs `.github/workflows/vn-pages.yml`, which renders
`vngen/build/story.play.json` into a static light-novel site with
`.vnstudio/pages/vn-site.mjs` and force-pushes the result to the `gh-pages` branch. Both of
those files are written by VN Studio's **Install GitHub Page Builder…** command; reinstall to
update them.

Serving the branch needs Settings ▸ Pages ▸ Deploy from a branch ▸ `gh-pages` ▸ `/ (root)`.
