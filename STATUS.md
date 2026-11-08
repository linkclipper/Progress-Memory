# STATUS — LinkClipper org

Updated: 2026-11-08

## Now

- **Phase B v1 shipped (code-complete, verified): board share links.** Self-contained snapshot in the fragment (`/b/#d=…`), public viewer live, schema v2, share modal, codec lib. v0.4.0 in manifest; release tag pending owner verification.
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

1. **Phase B — board share links** (`visibility: 'link'`, share slug, `linkclipper.github.io/b/<slug>` read-only page; RLS already drafted in `backend/supabase/schema.sql`).
2. Transient backend decision to record before any share link ships: anon-key write risk documented in backend README § Share.
3. Phase C later: hosted accounts + discovery (roadmap Phase C in product repo's `docs/ROADMAP.md`).
