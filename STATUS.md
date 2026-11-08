# STATUS — LinkClipper org

Updated: 2026-11-08

## Now

- **Phase B v1 in review:** static board share links work, and a discoverability fix (`ef49d9d`) makes Share visible in the selected-board toolbar and on sidebar boards. The initial release had put Share only inside an unreachable editor. v0.4.0 is in the manifest; release tag pending the owner's hands-on verification after reloading the unpacked extension.
- Store screenshots regenerated earlier today with photo thumbnails; published in `brand/` + site assets.
- Org structure complete: 13 live repos. All policy/process repos seeded with real content.

## Shipped (latest first)

- **v0.3.0** released: `LinkClipper-0.3.0.zip` on the GitHub release; CI green (`check & pack`, 19s); auto-release-from-tag proven.
- Reader feature (background fetch + extraction, per-site permission on click), YouTube floating window, Vimeo/IG/TikTok inline, `.hidden` bug fix, rebrand to LinkClipper.
- Schema versioning + migration ladder (`wc_meta`, `Store.MIGRATIONS`), board `visibility` reserved (`private` default).

## In flight

- None.

## Blocked (waiting on)

- **CWS listing submission** — blocked on owner's Chrome Web Store account actions: upload zip, fill data disclosure (privacy URL known: `https://linkclipper.github.io/privacy.html`), attach the 3 screenshots from `brand/webstore-screenshots/`, submit. Justifications ready in `Knowledgebase/runbooks/cws-submission.md`.

## Next (in order)

1. Owner: reload extension, select a board (including Inbox), click **Share board**, copy and open its snapshot link. Tag v0.4.0 only after this check.
2. Phase B2 live/revocable boards: resolve the anon-key write risk before sharing from a user-owned sync project. The v1 fragment snapshots neither change visibility nor require sync.
3. Phase C later: hosted accounts + discovery (roadmap Phase C in product repo's `docs/ROADMAP.md`).
