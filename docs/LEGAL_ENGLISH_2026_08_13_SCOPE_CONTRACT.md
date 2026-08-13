# Public legal English scope contract

## Intended behavior

The public Snuser legal and support pages must render in English at their
existing stable GitHub Pages URLs.

## Allowed files

- `index.html`
- `privacy-policy.html`
- `terms.html`
- `support.html`
- `docs/LEGAL_ENGLISH_2026_08_13_SCOPE_CONTRACT.md`

## Protected areas

- `app-ads.txt` and repository settings remain unchanged.
- Existing filenames, public URLs, relative navigation, contact email, adult-use
  notice, account-deletion route, provider disclosures, and legal meaning remain
  intact.
- No Snuser app code, backend, database, authentication configuration, or live
  user data is changed by this scope.

## Invariants

- Every page declares `lang="en"`, UTF-8, and a mobile viewport.
- Privacy and terms remain separate public documents.
- All pages link back to the legal index and retain
  `snuser.app@gmail.com` as the contact address.
- The translation must not weaken age, prohibited-use, privacy, moderation,
  account-deletion, liability, or third-party-service disclosures.

## Mandatory verification

- Inspect the complete diff and confirm that it is confined to the allowed files.
- Parse all four HTML files and verify their titles, headings, relative links,
  email links, and English language attributes.
- Search rendered copy for known Swedish navigation and section labels.
- After publishing, verify all four GitHub Pages URLs return HTTP 200 and render
  the expected English headings.
