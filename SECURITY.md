# Security Policy

This repository holds the source for **carolinaconde.com**, a static website
served via GitHub Pages. It has no backend, no database, no user accounts, and
collects no data — every page is plain HTML/CSS/JavaScript. As a result the
security surface is small, but responsible reports are always welcome.

## Reporting a vulnerability

If you find a security issue (for example an XSS vector in one of the pages, or
a compromised third‑party dependency), please report it privately:

- **Preferred:** open a report through GitHub's
  [Private vulnerability reporting](https://github.com/ccondeo/carolinaconde.com/security/advisories/new)
  (Security → Report a vulnerability).
- **Email:** translator@carolinaconde.com

Please include the affected page or file, a description of the issue, and steps
to reproduce. Do **not** open a public issue for a security vulnerability.

You can expect an acknowledgement within a few days. Since this is a personal
site maintained by one person, timelines are best‑effort.

## Scope

In scope:

- The pages served from this repository (`index.html` and everything under
  `work/`).

Out of scope:

- GitHub Pages infrastructure itself (report those to
  [GitHub](https://bounty.github.com/)).
- Third‑party services the pages link to or load (e.g. Google Fonts, jsDelivr).
  If a loaded dependency is compromised, that's worth reporting here so the
  reference can be removed or pinned.

## Third‑party dependencies

The site is intentionally dependency‑light. The only external runtime assets are
web fonts (Google Fonts) and, on the glossary page, an icon font loaded from a
CDN (jsDelivr). There is no build step and no package manager.
