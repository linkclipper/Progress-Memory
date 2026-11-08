# STATUS — LinkClipper org

Updated: 2026-11-08

## Now

- Store screenshots (grid / reader / edit) regenerated with photo thumbnails and verified; published to `linkclipper.github.io/assets/`, `brand/webstore-screenshots/`.
- Org structure complete: 13 live repos — product, Knowledgebase, backend, brand, design-system, Progress-Memory, Workflows, Security-Trust, Monetization, Marketing, Data-Analytics, linkclipper.github.io + .github profile. All policy/process repos seeded with real content (business model ban list, launch plan, threat model, procedures, zero-telemetry law).

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
