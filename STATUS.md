# STATUS — LinkClipper org

Updated: 2026-11-11

## Now

- **Local AI access phase 1** on `main` at `e3e41e9`: dashboard **✦ AI** panel exports a reviewed snapshot and applies staged AI changes; `mcp/` contains a dependency-free stdio MCP server plus a `127.0.0.1` bearer-token HTTP API. Tools cover search/read plus create/update/move/delete, but AI writes land in `linkclipper-changes.json` and only change the library after the user reviews them in the dashboard. 34 Node tests and check & pack run `42921647774` pass. `mcp/` is deliberately excluded from the store zip.
- **Unreleased social capture work** is still on `main` behind v0.4.0: X post-scoped media/source marks (`7df58ba`), Reddit Save beside Share (`8363a2d`..`b0d0a97`), and Instagram/TikTok controls plus grid badges (`1743493`). Not in the published v0.4.0 zip.
- **v0.4.0 released** after owner hands-on confirmation. Tag `v0.4.0` points to product `f654f76`; check & pack CI and tag-triggered release CI passed. Public release includes `LinkClipper-0.4.0.zip`; downloaded artifact verified against the GitHub SHA-256 digest, manifest version, required files and exclusion of the dev harness.
- The release includes static board snapshot sharing, explicit duplicate choices, bulk collection tools, quick-save and palette shortcuts, local profile, dashboard polish and the linked-loop mark. Core use remains account-free and local-first; snapshot links cannot be revoked.
- Landing page update `be671fe` replaces preview messaging with v0.4.0 release copy; Pages deployment `42510118188` passed and live content was checked.
- The 13-repo organization remains populated; product and brand assets, documentation and policies are maintained separately.

## Blocked (waiting on)

- **Chrome Web Store submission** requires owner account actions: upload the next release zip, complete data disclosure, attach current screenshots from `brand/webstore-screenshots/`, and submit. Privacy URL: `https://linkclipper.github.io/privacy.html`. Justifications: `Knowledgebase/runbooks/cws-submission.md`.
- **MCP distribution** is unresolved: `mcp/` is not in the Chrome Web Store package. A user who installs only from the store must clone/download the repository to run the AI server unless a standalone package or release asset is published.

## Next

1. Owner live check after reloading the unpacked extension: X posts with and without media, Reddit Save beside Share, Instagram post/reel actions and grid badges, TikTok action rail. TikTok was unreachable from the build machine, so its `data-e2e` adapter is selector-tested only.
2. Exercise AI phase 1 with a real client: Claude Desktop or Cursor over stdio, and one local-LLM adapter over HTTP. Export, search, stage each operation type, review/apply in the dashboard, and verify a changed-since-snapshot conflict is skipped.
3. Improve MCP distribution: publish a standalone `linkclipper-mcp` package or attach a versioned server zip to GitHub releases, then point the dashboard panel at it.
4. Cut the next release from `main` — recommend 0.5.0 (social save controls + AI panel) — then use that artifact for the Chrome Web Store listing and refreshed linked-loop screenshots.
5. Phase 2 AI: live bridge with real-time reads, direct writes behind per-tool permissions, and an optional on-device embedding index. Keep the phase-1 tool names and JSON shapes stable.
6. Phase B2 live/revocable boards only after resolving the anon-key write risk. v1 snapshots remain static and non-revocable.
