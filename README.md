**Senior Android Engineer.** Kotlin, Jetpack Compose, and 20+ years building production software.

Currently building **Elsie**, an accessibility-focused Android launcher for older adults and the visually impaired, with a caregiver companion app that sets it up and watches over it remotely. It's live on [Google Play](https://play.google.com/store/apps/details?id=com.fangjet.launcher), and you can read more at [elsiefamily.com](https://www.elsiefamily.com).

I use AI-assisted tooling such as Claude Code and Gemini daily for implementation, testing, and debugging, held to the same standard as anything else I ship. My projects are mostly Android, though there's iOS (Swift/SwiftUI) and PHP work below too.

You can read more at [fangjet.com](https://www.fangjet.com) and [LinkedIn](https://www.linkedin.com/in/colin-r-tucker/).

Public Projects
---

**[Sunny & Misty](https://github.com/tuckercr/weather-android)**: A pet weather app built natively twice, for [Android](https://github.com/tuckercr/weather-android) (Kotlin/Compose) and [iOS](https://github.com/tuckercr/weather-iOS) (Swift/SwiftUI). Sunny the dog and Misty the cat act out the forecast and suggest the best time for a walk. Multiple saved cities, one-tap current location, multi-day forecasts with tappable day details, animated radar, and scheduled daily briefings. Per-city caching paints instantly and refreshes in the background, falling back to cached data when the network fails. The iOS app has recently caught up with Android on settings, radar, notifications, and background refresh, and now shows sunrise and sunset in each city's own time zone. Feature switches and walk-safety thresholds are tunable from Remote Config without shipping a build. Offline-first · MVVM + Hilt · WorkManager · Material 3 · Firebase Analytics/Remote Config/Crashlytics · GitHub Actions CI.

**[Hark](https://github.com/tuckercr/wakewordapp)**: On-device wake-word detection using PocketSphinx, with no cloud and no network dependency. An earlier proof-of-concept, built to help hearing-impaired users notice when they're being addressed, and my most starred and forked project.


Client & Private Work
---

Production source is private, although Rolo has a public showcase.

**[Elsie](https://www.elsiefamily.com)**: A two-app accessibility product, available on [Google Play](https://play.google.com/store/apps/details?id=com.fangjet.launcher). A Compose launcher with large touch targets, fall detection, medication reminders, voice commands, and a usage-ranked row of real apps with notification dots. A caregiver app pairs by 6-digit code and manages the phone remotely: contacts edited on one phone land on the other within seconds, with Firestore security rules enforcing which side owns what. Safety timings are tunable from Remote Config without shipping a build. Multi-module Kotlin · Firebase Auth/Firestore/Remote Config · GitHub Actions CI.

**[Rolo](https://github.com/tuckercr/rolo-showcase)**: A relationship-first CRM built for a fractional CMO consultancy, replacing a spreadsheet. A configurable follow-up rules engine schedules each contact's next touch from per-stage cadence rules; a dashboard surfaces overdue and due-this-week, and a scheduled daily digest email reports what's due and what was logged yesterday. Interaction history with edit-in-place, snooze, and soft delete. An MCP connector lets AI assistants such as Claude search contacts and activity, while every write is queued as a proposal that a human approves in Rolo. PHP 8.4 · MariaDB · MCP · server-rendered, no build pipeline.

**Commercial Translation Diagnostic**: A paid AI analysis product. Clients upload a pitch deck and supporting documents and complete a survey; Claude drafts a findings report that a human reviews before it reaches the client. It also reads the company's own website, following the sitemap and internal links, recovering copy from the script files of JavaScript-rendered sites, and falling back to Firecrawl when a site blocks requests from a data center. Client-supplied URLs are fetched with SSRF protection (every redirect re-checked and pinned to a public IP), and Claude's output is schema-constrained and validated before anyone sees it. PHP 8.4 · Claude API · Stripe · Firecrawl.
