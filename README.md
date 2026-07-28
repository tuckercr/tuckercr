**Senior Android Engineer** — Kotlin, Jetpack Compose, and 20+ years building production software.

Currently building **EasyLink** — an accessibility-focused Android launcher for older adults and the visually impaired, a caregiver companion app that sets it up and watches over it remotely, and [easylinkcare.com](https://easylinkcare.com), a Firebase-hosted site with a Firestore-backed waitlist. All three deploy from the same repo.

I use AI-assisted tooling such as Claude Code and Gemini daily for implementation, testing, and debugging, held to the same standard as anything else I ship.  My Projects are mostly Android, though there's iOS (Swift/SwiftUI) and PHP work below too.

You can read more at [fangjet.com](https://www.fangjet.com) and [LinkedIn](https://www.linkedin.com/in/colin-r-tucker/).

Public Projects
---

**[EasyLink](https://github.com/tuckercr/easylink)** — Two-app accessibility product. A Compose launcher with large touch targets, hold-to-activate SOS, fall detection, medication reminders, voice commands, and a usage-ranked row of real apps with notification dots. A caregiver app pairs by 6-digit code and manages the phone remotely — contacts edited on one phone land on the other within seconds, with Firestore security rules enforcing which side owns what. Safety timings like the SOS hold and countdown are tunable from Remote Config without shipping a build. Multi-module Kotlin · Firebase Auth/Firestore/Remote Config · 260+ unit tests · GitHub Actions CI.

**[Cats & Dogs](https://github.com/tuckercr/cats-dogs)** — A weather app built natively twice: [Android](https://github.com/tuckercr/cats-dogs) (Kotlin/Compose) and [iOS](https://github.com/tuckercr/cats-dogs-iOS) (Swift/SwiftUI). Swipeable saved cities, multi-day forecasts, embedded radar, and daily briefings scheduled with WorkManager. Offline-first · MVVM + Hilt · Material 3 · Firebase Analytics/Remote Config.

**[ZamZow](https://github.com/tuckercr/wakewordapp)** — On-device wake-word detection using PocketSphinx: no cloud, no network dependency. An earlier proof-of-concept, built to help hearing-impaired users notice when they're being addressed — and my most starred and forked project.


Client & Private Work
---

Production source is private, although Rolo has a public showcase.

**[Rolo](https://github.com/tuckercr/rolo-showcase)** — A relationship-first CRM built for a fractional CMO consultancy, replacing a spreadsheet. A configurable follow-up rules engine schedules each contact's next touch from per-stage cadence rules; a dashboard surfaces overdue and due-this-week, and a scheduled daily digest email reports what's due and what was logged yesterday. Interaction history with edit-in-place, snooze, and soft delete. PHP 8.4 · MariaDB · server-rendered, no build pipeline · 400+ file PHPUnit suite.

**Commercial Translation Diagnostic** — A paid AI analysis product. Clients pay through Stripe, upload a pitch deck and supporting documents, and complete a survey; the system parses PDF/Word/PowerPoint, runs the analysis, and drafts a report for human review before it reaches the client. PHP 8.4 · Stripe · 440+ file PHPUnit suite.
