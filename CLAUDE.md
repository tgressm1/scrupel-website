# Brand consistency with the main app

This site mirrors its brand from a separate, unrelated repo — `../my-app`
(sibling directory, own git repo, own Claude Code session), which is the
**canonical source of brand truth**. That's the real Scrupel product; this
site is derivative marketing collateral.

Specifically mirrored from there:

- **Color palette**: this repo's `styles.css` `:root` (light) and
  `@media (prefers-color-scheme: dark)` blocks are hand-copied from
  `../my-app/src/App.jsx`'s `LIGHT`/`DARK` theme objects.
- **Favicon**: `favicon.png` here is a copy of
  `../my-app/android/app/src/main/res/mipmap-xxxhdpi/ic_launcher.png`.
- **Feature copy** in `index.html`: describes what the app actually does —
  should stay accurate to the real feature set in `../my-app`.

**If asked to change colors, the icon, or feature copy here**, first check
whether `../my-app` changed first (read it directly). If the app changed
and this site hasn't caught up, pull the new values across in the same
turn — don't ask the user to manually copy anything between chats. If
nothing changed on the app side, this is probably a one-off, site-only
tweak (e.g. pure copywriting/layout) and doesn't need to touch `../my-app`
at all.

# Workflow

Wait for an explicit "Go" (or clear equivalent) before committing or
pushing — make the change, then stop and report what changed rather than
committing in the same turn. This mirrors the standing convention already
established in `../my-app`; it's a general preference for how Tyler works,
not something specific to that repo.
