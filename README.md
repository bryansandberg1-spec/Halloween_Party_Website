# Halloween_Party_Website

Sandberg Halloween Party — October 24, 2026.

## Files

- `index.html` — the whole site, self-contained (no build step, no dependencies).
- `CNAME` — the custom domain for GitHub Pages.
- `Sandberg Party Site.dc.html` + `media/` — the editable source this site is generated from.

## Hosting on GitHub Pages

1. Repo **Settings → Pages**.
2. Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
3. Under **Custom domain**, enter your GoDaddy domain and save. `CNAME` already holds it.
4. Check **Enforce HTTPS** once the certificate is issued (can take an hour).

Note: GitHub Pages on a **private** repository requires a paid plan. Make the repo public, or upgrade, or host the same `index.html` on Netlify for free.

## GoDaddy DNS

In GoDaddy → your domain → DNS, set:

| Type  | Name | Value |
|-------|------|-------|
| A     | @    | 185.199.108.153 |
| A     | @    | 185.199.109.153 |
| A     | @    | 185.199.110.153 |
| A     | @    | 185.199.111.153 |
| CNAME | www  | bryansandberg1-spec.github.io |

DNS can take a few hours to propagate.

## Editing the site

Open the site, click **Edit site**, sign in (`mohsandy`). Every field, list, guest,
potluck slot, and the theme are editable there. Content saves in your browser and can be
exported as JSON. To make an edit permanent for all visitors, re-generate `index.html`
from the source file.

## RSVPs

RSVPs, potluck claims, and signup requests open a pre-filled email to
**sandberghalloween@gmail.com**. Guest-side changes save only in that guest's own browser —
the emails are what reaches you. Keep the master list in the editor's Guests tab
(CSV import/export, copy all emails, open Gmail to all).
