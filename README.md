# KalingApp — Mobile App Downloads

Debug builds of the KalingApp mobile application, published here so they can be
installed on a phone without needing access to the source repository.

## Download

**[kalingapp-v1.0-debug.apk](kalingapp-v1.0-debug.apk)** — 20.9 MiB

Updated 2026-10-07 (4): discarding the donor questionnaire now sticks. The form
fills itself in from your last submission; after you confirmed "discard" it
used to stay blank for only the next open, then your old answers came back.
They now stay gone, including after closing the app. Resubmitting a declined
request still brings your answers back. Same signing certificate as the
previous build.

Previous update (2026-10-07, 3): every booking now starts by asking whether to update your
location, so you always know it is being brought up to where you are now. If it
can't be read (permission, location off, no signal), the app tells you it will
use your saved location instead and lets you continue. Same signing
certificate as the previous build.

Previous update (2026-10-07, 2): the app now looks the same on tablets as on phones. The
layout stays phone-width and centred instead of stretching edge to edge, and
the onboarding card is properly centred. Same signing certificate as the
previous build.

Previous update (2026-10-07): the appointment scheduler no longer offers a 5:00 PM slot
(last slot is now 4:00 PM), for both donors and recipients. Same signing
certificate as the previous build.

Previous update (2026-10-06, 2): the app's descriptions and hints are now one short,
plain sentence each (Milk Bank intro, onboarding, the guided tour, FAQ and
Help). Same signing certificate as the previous build.

Previous update (2026-10-06): the phone's back button and back gesture no longer close
the whole app. They go back one screen, and the gesture slides the screen as
you drag. Pull down to refresh now also works on Knowledge Hub, Saved
Articles, Notifications, Transaction History, Booking Status and the Contact
Directory. Same signing certificate as the previous build.

Previous update (2026-10-02): the Request Milk form now asks "Leave without
saving?" when you tap back after filling anything in, the same way the
donor questionnaire does, instead of leaving straight away. The phone's
own back button/gesture goes through the same prompt (it used to close
the app from that screen). Also: the Contact Directory now shows each
organization's email, tappable to open your mail app, and lists
Quezon City General Hospital and St. Luke's Medical Center - Quezon
City alongside Fabella and Arugaan. Same signing certificate as the
previous build.

Previous update (2026-10-01, 2): the Request Milk form's requirements checklist
(baby's name, clinic notes, prescription proof, cooler, medical
abstract) is now actually sent when you submit a recipient request.
Previously the form collected and validated all of it on-screen, then
silently threw it away the moment the booking was created — the
facility never received any of it, for any recipient request, ever.
Same signing certificate as the previous build.

Previous update (2026-10-01): discarding the donor questionnaire (the "Leave
without saving?" prompt) now actually stays discarded. Previously, if
you'd ever submitted a real questionnaire before, reopening the form
right after discarding would quietly refill it with that old
submission again — the discard itself worked, but the very next open
silently undid it, which looked exactly like Discard doing nothing.
Also: the article detail screen no longer shows a star rating next to
the category tag (it never did anything), and the spacing above that
tag was tightened so it no longer looks like it's sitting on its own
detached line. Same signing certificate as the previous build.

Previous update (2026-09-30, fix): the previous fix wired the questionnaire
pre-fill into the wrong entry point. "Submit a New Request" on a
declined booking was skipping the questionnaire screen entirely --
resubmitting created a new request with no questionnaire attached at
all, not just a blank one. Fixed for real this time: resubmitting a
donor request now goes back through the (pre-filled) questionnaire
screen before scheduling. Same signing certificate as the previous
build, so installing over it works without uninstalling first.

Previous update (2026-09-30): resubmitting a donor request after a
decline no longer forces a blank questionnaire -- her last answers are
pre-filled, with a notice to review them (and re-attach her serology
photo) before submitting.

Previous update (2026-09-29): the app now points at the new Singapore
backend (backend-kalingapp.onrender.com, co-located with the Supabase
database) instead of the old Oregon one.

Previous update (also 2026-09-29): Transaction History now shows the
millilitres donated/received on each entry; the appointment scheduler no
longer lets you pick a date before today (a timezone bug, only visible
before 8 AM Philippine time); and a same-day booking now grays out time
slots that have already passed.

Previous update (also 2026-09-29): fixed the Forgot Password screen
showing "Resetting…" before you'd touched it, and "Sending…" stuck
after tapping back.

On a phone, tap the link above, then tap **Download**. Open the file when it
finishes and Android will ask to install it.

## Installing

This is a debug build signed with Android's standard debug certificate, not a
Play Store release, so Android will warn you before installing it. That warning
is expected.

1. Download the APK using the link above.
2. Open it. Android will say installs from this source are blocked.
3. Tap **Settings**, turn on **Allow from this source**, then go back.
4. Tap **Install**.

If you previously installed a build signed with a different key, uninstall the
old copy first — Android refuses to replace an app when the signing certificate
does not match.

## This build

| | |
|---|---|
| Version | 1.0 (versionCode 1) |
| Package | `com.aistudio.kalingapp.hsmqwr` |
| Requires | Android 7.0 (API 24) or newer |
| Built against | Android API 36 |
| Size | 21,879,335 bytes |
| SHA-256 | `c33fbfdba163aabe74927a15f8d1ba08010adf6731115db7f30dbf92733d7241` |
| Signing | Debug certificate, V2 scheme (SHA-256 `a2b8…3b5e`) |
| Source commit | `KalingApp-Prototype@7516521` |

To confirm the file downloaded intact, compare the SHA-256:

```bash
sha256sum kalingapp-v1.0-debug.apk        # Linux / macOS / Git Bash
certutil -hashfile kalingapp-v1.0-debug.apk SHA256   # Windows
```

## Notes

Milk volumes throughout the app are millilitres. The admin console displays
facility stock in litres, but that is display formatting over the same stored
millilitres — there is no second unit anywhere in the system.

The app talks to the live backend on Render, which sleeps after 15 minutes of
inactivity on the free plan. The first request after a quiet period can take
10–30 seconds while the server wakes up. That is expected, not a failure.

This repository holds built artifacts only. The application source lives in a
separate, private repository.
