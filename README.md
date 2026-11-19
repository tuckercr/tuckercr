**Senior Android Engineer.** Kotlin, Jetpack Compose, and 20+ years building production software. Based near Knoxville, TN, and open to senior and staff mobile roles.

I build and ship my own apps end to end. **Elsie**, an accessibility launcher for older adults, is live on [Google Play](https://play.google.com/store/apps/details?id=com.fangjet.launcher). **Sunny & Misty**, a pet weather app built natively for both platforms, is live on [Google Play](https://play.google.com/store/apps/details?id=com.fangjet.weather) and the [App Store](https://apps.apple.com/app/id6827945995).

I use AI agents such as Claude Code and Gemini daily for implementation, testing, and debugging, set up per project and held to the same standard as anything else I ship. [How I use AI](https://fangjet.com/ai) covers the setup, an MCP server I built, and the local models I've tested.

**[fangjet.com](https://fangjet.com)** · [Projects](https://fangjet.com/projects) · [Résumé](https://fangjet.com/colin-tucker-resume.pdf) · [LinkedIn](https://www.linkedin.com/in/colin-r-tucker/) · [colin@fangjet.com](mailto:colin@fangjet.com)

Shipped Apps
---

**Sunny & Misty** · [sunnyandmisty.com](https://sunnyandmisty.com) · [Google Play](https://play.google.com/store/apps/details?id=com.fangjet.weather) · [App Store](https://apps.apple.com/app/id6827945995) · source for [Android](https://github.com/tuckercr/weather-android) and [iOS](https://github.com/tuckercr/weather-iOS)

A weather app where Sunny the dog and Misty the cat act out the forecast and suggest the best time for a walk, built natively twice: Kotlin/Compose for Android, Swift/SwiftUI for iOS. Multiple saved cities, one-tap current location, multi-day forecasts with tappable day details, animated radar, and scheduled daily briefings. Offline-first: per-city caching paints instantly and refreshes in the background, falling back to cached data when the network fails. Feature switches and walk-safety thresholds are tunable from Remote Config without shipping a build. 780+ unit tests and Compose UI tests on Android, 720+ XCTest tests on iOS. MVVM + Hilt · WorkManager · Material 3 · SwiftUI · Firebase Analytics/Remote Config/Crashlytics · GitHub Actions CI.

**Elsie** · [elsiefamily.com](https://www.elsiefamily.com) · [Google Play](https://play.google.com/store/apps/details?id=com.fangjet.launcher) · private source

An Android launcher for older adults and people with low vision, paired with a caregiver app that sets it up and manages it remotely. The launcher stays simple and legible: large color-coded buttons, medication reminders, voice commands, a magnifier, photo speed dial, and a usage-ranked row of real apps with notification dots. The caregiver app, Elsie Family, pairs with a 6-digit code: contacts edited on one phone land on the other within seconds, with Firestore security rules enforcing which side owns what. Both apps live in one multi-module Kotlin codebase with shared contracts, and safety timings are tunable from Remote Config. 740+ unit tests and Compose UI tests. Kotlin · Compose · Hilt · Room · Firebase Auth/Firestore/Remote Config · GitHub Actions CI.

Open Source
---

**[Hark](https://github.com/tuckercr/wakewordapp)**: Fully on-device wake-word detection for Android using PocketSphinx, with no cloud and no network dependency. Built to help hearing-impaired users notice when they're being addressed. Runs as a microphone foreground service that handles Android 14's background and boot restrictions, with multi-word phrases, tunable sensitivity, and a custom alert sound and duration. My most starred and forked project.

**[fangjet.com](https://github.com/tuckercr/fangjet)**: My portfolio site, rebuilt from WordPress in React and Vite, with every page prerendered to static HTML. MIT licensed.

Client Work
---

Production source is private, although Rolo has a public showcase.

**[Rolo](https://github.com/tuckercr/rolo-showcase)**: A relationship-first CRM for Data Story Strategy, a two-person consultancy, running their client pipeline in production since July 2026. It decides who you owe a follow-up and comes to find you, rather than waiting to be opened.

- **Follow-up engine.** Configurable per-stage cadence rules schedule each contact's next touch; a dashboard and a daily digest email surface what's overdue and due this week.
- **MCP server.** AI assistants such as Claude search contacts and activity over the Model Context Protocol. Agents can propose any change, but every write is queued until a human approves it on a before/after diff.
- **Slack bot.** A weekday 5 PM debrief DMs the contacts you owe, with Log, Open, Snooze, and Skip buttons and a 10-second logging modal. A `/rolo` command handles lookups and quick logs, a Monday alert catches contacts going cold, and an optional Google Calendar connection offers to log the meetings you actually had.
- **Built to run anywhere.** Plain PHP 8.4 and MariaDB, server-rendered, on shared hosting: signed webhooks in, API calls out, no resident process and no build step.

PHP 8.4 · MariaDB · PHPUnit · MCP · Slack API · Google Calendar API.

**Commercial Translation Diagnostic**: A paid AI analysis product for the same consultancy. Clients complete a structured intake and upload a pitch deck and supporting documents; the system also reads their website, then Claude drafts a findings report that a consultant reviews and edits before the client sees it. The website reader follows the sitemap and internal links, recovers copy from JavaScript-rendered sites, and falls back to Firecrawl when a site blocks data-center requests. Client-supplied URLs are fetched with SSRF protection (every redirect re-checked and pinned to a public IP), and Claude's output is schema-constrained and validated before anyone sees it. Stripe checkout, Google Sign-In for admins, and automatic retry and alerting when generation fails. PHP 8.4 · Claude API · Stripe · Firecrawl.

**Whiteboard Camera**: An Android prototype that removes the presenter from a whiteboard video in real time with OpenCV and the NDK, then streams the cleaned-up feed to conferencing platforms. The result looks like writing appearing on the board with no one in front of it. Kotlin · OpenCV · Android NDK · Camera2 · WebRTC · RTMP.
