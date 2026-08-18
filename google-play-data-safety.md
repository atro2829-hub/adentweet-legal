# AdenTweet — Google Play Data Safety Draft

**Status:** Release-preparation draft, reviewed against the implemented product features on August 18, 2026. This document is not a substitute for completing the Play Console questionnaire against the final production build, SDK inventory, service providers, and actual operational practices.

| Play Console topic | Proposed disclosure for the current build | Implementation basis |
|---|---|---|
| Data collected | Name, email address, user IDs, public profile information, posts and media, direct messages, anonymous-message content, moderation reports, verification information, app/device/session data, and interaction events. | Local account flow, profiles, content, messaging, Sarahni, moderation, and session handling. |
| Data shared | Do **not** declare data as “sold.” Declare sharing only if production providers receive data outside the service operator’s behalf; re-evaluate every hosting, analytics, crash-reporting, advertising, and support SDK before submission. | Service uses managed backend, storage, and authentication services. |
| Purpose | App functionality, account management, security/fraud prevention, moderation, communications, and analytics/feature performance when enabled. | Social feed, notifications, security controls, and aggregate post views. |
| Security practices | Data is transmitted through secure network connections in production. Confirm any encryption-at-rest claim with the deployed provider before marking it in Play Console. | Do not overclaim beyond verified production configuration. |
| Deletion | User can request deletion at the public data-deletion URL; account verification is required before action. | `data-deletion.html` and in-app privacy path. |
| Optionality | Public profile fields and content are user-provided; privacy controls include anonymous-message availability. Required account fields should be marked accurately in the questionnaire. | Registration and profile settings. |

## Final submission checks

1. Inspect every production dependency and SDK, including any analytics, advertising, crash reporting, authentication, and payment package, and update Data Safety answers for the final build.
2. Publish the privacy-policy URL on a publicly accessible, non-geofenced page and add the same URL to Play Console and the application.
3. Complete the Content Rating questionnaire honestly, based on user-generated content, messaging, reporting, and moderation controls.
4. Complete the App Access form with instructions and valid review credentials if any feature is gated by sign-in.
5. Complete Ads, Target Audience, Government Apps, Financial Features, Data Deletion, and permissions declarations based on the final shipped behavior.
6. Re-check all disclosures after each release that adds an SDK, data category, external provider, or new use of data.

## Official references

1. [Google Play User Data policy](https://support.google.com/googleplay/android-developer/answer/10144311?hl=en)
2. [Google Play Data safety form](https://support.google.com/googleplay/android-developer/answer/10787469?hl=en)
3. [Google Play account deletion requirements](https://support.google.com/googleplay/android-developer/answer/13327111?hl=en)
