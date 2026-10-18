# KalingApp — Mobile App Downloads

Debug builds of the KalingApp mobile application, published here so they can be
installed on a phone without needing access to the source repository.

## Download

**[kalingapp-v1.0-debug.apk](kalingapp-v1.0-debug.apk)** — 22.7 MiB

Updated 2026-10-19 (3): when requesting pasteurized milk, you now say how much
you need after you are matched with a milk bank, on the scheduling screen,
within that milk bank's own limits. If the milk bank dispenses milk in bottles,
you can ask in bottles or in mL (Philippine milk bank bottles are a standard
100 mL, so 1 bottle = 100 mL). Booking Status shows your request the way you
made it, e.g. "3 bottles (300 mL)". Same signing certificate as the previous
build.

Previous update (2026-10-19, 2): tapping Donate Milk or Request Pasteurized Milk now
shows, after the reminder, a "What happens next" window with each step of the
Booking Tracker and one line on what happens in it, so the tracker is already
familiar once you submit. The app walkthrough is readable again: its cards
had turned see-through over the dimmed screen. Same signing certificate as the
previous build.

Previous update (2026-10-19): the glass cards are more see-through, closer to clear
glass, and the colours behind them now visibly flow around the screen (they
hold still if "Remove animations" is turned on in your phone's accessibility
settings). Pink and gold headings and labels are a deeper shade so they are
easy to read on the glass. The bottom menu is rebuilt: the highlight on the
selected tab no longer spills past the menu's rounded ends, and "Knowledge"
stays on one line, the same size as the other labels. On the home screen the
streak card's "Active Postpartum Journey" label sits above the title instead
of in its own box, the icon squares are see-through, and a 1-day streak says
"1 day". Text fields no longer put a box around their label, and Kali's
answers now have a "Read in Knowledge Hub" button under each article Kali
cites. Same signing certificate as the previous build.

Previous update (2026-10-13, 3): the glass look is now clear glass. Cards are see-through
panes with a bright edge and a soft shadow, and the light on them moves as you
tilt your phone. The colours behind the glass drift slowly too. The bottom menu
is a floating glass capsule. The pink is back to the original shade. Same
signing certificate as the previous build.

Previous update (2026-10-13, 2): a new look. Screens now have a frosted-glass style on a
soft pink, gold and lilac background, with a deeper pink that is easier to read.
While a page is loading you now see its outline shimmering in place instead of a
blank screen or a "nothing here" message. Same signing certificate as the
previous build.

Previous update (2026-10-13): saved articles now stay saved. They are stored on your
account, so they are still there after you sign out and back in, reinstall, or
switch phones. Sign-in is safer: after 3 wrong passwords the login screen
suggests resetting your password, and after 5 the account is locked for longer
and longer, with a countdown and who to contact. A strip at the top says "No
internet connection" while you are offline and "Back online" when it returns.
The sign-up and password-reset codes are entered one digit per box. Donate Milk
and Request Pasteurized Milk now show a short reminder of what you will need
before the form opens. The Knowledge Hub shows Educational Videos & Guides added
by the admin. Same signing certificate as the previous build.

Previous update (2026-10-07, 6): "Your Facility" now always appears on the scheduler and the
booking tracker. It could be missing for a whole session if the app was opened while
the server was still waking up; the facility chosen for you is now kept as soon as
the server returns it, and pulling down to refresh reloads it. Same signing
certificate as the previous build.

Previous update (2026-10-07, 5): the home screen no longer shows the "Care Track • N Weeks
Old" line under the greeting. Nothing else on the screen changed. Same signing
certificate as the previous build.

Previous update (2026-10-07, 4): discarding the donor questionnaire now sticks. The form
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
| Size | 23,789,397 bytes |
| SHA-256 | `d63b81838ef82f8cb4a05e51d212d011413e88784a4115cb0f3f23e0c81d1992` |
| Signing | Debug certificate, V2 scheme (SHA-256 `a2b8…3b5e`) |
| Source commit | `KalingApp-Prototype@5619090` |

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
