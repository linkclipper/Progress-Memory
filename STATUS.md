# STATUS — LinkClipper org

Updated: 2026-11-09

## Now

- **Unreleased social capture work** on `main` at `1743493` (product manifest still 0.4.0): X post-scoped media and offline source marks (`7df58ba`), Reddit explicit save button in the post action row beside Share (`8363a2d`..`b0d0a97`), and Instagram/TikTok save controls plus grid badges (`1743493`). 27 Node tests and check & pack run `42672235055` pass. Not in the published v0.4.0 zip.
- **v0.4.0 released** after owner hands-on confirmation. Tag `v0.4.0` points to product `f654f76`; check & pack CI and tag-triggered release CI passed. Public release includes `LinkClipper-0.4.0.zip`; downloaded artifact verified against the GitHub SHA-256 digest, manifest version, required files and exclusion of the dev harness.
- The release includes static board snapshot sharing, explicit duplicate choices, bulk collection tools, quick-save and palette shortcuts, local profile, dashboard polish and the linked-loop mark. Core use remains account-free and local-first; snapshot links cannot be revoked.
- Landing page update `be671fe` replaces preview messaging with v0.4.0 release copy; Pages deployment `42510118188` passed and live content was checked.
- The 13-repo organization remains populated; product and brand assets, documentation and policies are maintained separately.

## Blocked (waiting on)

- **Chrome Web Store submission** requires owner account actions: upload the v0.4.0 zip, complete data disclosure, attach current screenshots from `brand/webstore-screenshots/`, and submit. Privacy URL: `https://linkclipper.github.io/privacy.html`. Justifications: `Knowledgebase/runbooks/cws-submission.md`.

## Next

1. Owner live check after reloading the unpacked extension: X posts with and without media, Reddit Save beside Share, Instagram post/reel actions and grid badges, TikTok action rail. TikTok was unreachable from the build machine, so its `data-e2e` adapter is selector-tested only.
2. Cut v0.4.1 with the unreleased social work, then use that artifact for the Chrome Web Store listing and refreshed linked-loop screenshots; submission requires owner account access.
3. Phase B2 live/revocable boards only after resolving the anon-key write risk. v1 snapshots remain static and non-revocable.
4. Phase C later: hosted accounts and discovery, while offline core remains independent (see product `docs/ROADMAP.md`).
