# AdenTweet Legal Pages

Official public-facing legal pages for AdenTweet by Mohammed Al-Qutaibi / QTBM DEV.

The site contains privacy, terms, community guidelines, and contact pages. It is intentionally static and never contains Supabase service-role credentials. The Android application remains the source of authenticated data and reads only public organization/legal configuration. Any update to organization settings should be reviewed and published through the controlled GitHub workflow.

## Pages

- `index.html` — legal hub
- `privacy.html` — privacy notice
- `terms.html` — terms of use
- `community-guidelines.html` — safety standards
- `contact.html` — support contact

## Publishing

This repository is prepared for GitHub Pages. Before public release, set the final repository visibility and Pages source in GitHub, then place the resulting public URL in the Supabase `app_settings` record and the Android app configuration. Do not expose private tokens in static files.
