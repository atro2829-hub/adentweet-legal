# AdenTweet Legal Center

This repository contains the public-facing legal pages and Google Play release-preparation materials for AdenTweet.

| Public page | Purpose |
|---|---|
| `privacy.html` | Privacy Policy and data-processing disclosure |
| `terms.html` | Terms of Use |
| `community-guidelines.html` | Content, safety, and moderation standards |
| `data-deletion.html` | Account and data deletion instructions |
| `contact.html` | Privacy, safety, and legal contact channel |
| `google-play-data-safety.md` | Draft Data Safety and release checklist for Play Console |

## Publication

This repository is public. Enable GitHub Pages from the default branch and use the resulting HTTPS address as the public privacy-policy URL. After Pages is live, set `homepageUrl` to the legal hub and update the `ADENTWEET_LEGAL_URL` value in the mobile project to that exact public URL. Do not publish secrets, OAuth credentials, database URLs, production review credentials, or private user data in this repository.

## Review note

These are working documents for legal and operational review. Update them before release when the production domain, business entity, support email, retention requirements, third-party SDKs, advertising status, or data flows change.
