---
layout: default
title: Privacy Policy
permalink: /privacy
---

# Privacy Policy

**Last updated: October 2, 2026**

Readglide is a teleprompter for iPhone and iPad made by Kohei Omori, a sole proprietor based in Japan (called "the developer" below). Rather than listing categories of data, this page walks through the app in the order you use it (writing a script, reading and recording, reviewing a take, exporting) and says at each stage what Readglide keeps, where, and when it goes away. None of it reaches the developer: Readglide has no server, no account and no network code, and it collects no personal information.

---

## Stage 1: writing a script

The scripts you type, paste or import, and your display and scrolling preferences, are written to Readglide's own storage on your iPhone or iPad. They are not uploaded anywhere, neither to the developer nor to any other company.

Two of Apple's "required reason" APIs are used at this stage, both purely on the device: user defaults (reason CA92.1) hold your preferences, and file timestamps (reason C617.1) let the library list and re-index saved scripts.

## Stage 2: reading, recording and practicing aloud

Scrolling a script needs no permission at all. Each optional feature below asks iOS for one permission, with an explanation, the first time you use it; saying no switches off only that feature. Readglide never asks for location, contacts or notifications.

- **Camera** (`NSCameraUsageDescription`): filming while the script is on screen. The video is recorded on the device and goes nowhere else.
- **Microphone** (`NSMicrophoneUsageDescription`): sound for a video, and practice with audio only. Sound is written only into that video or that practice recording and is not transmitted. Practice recordings are never added to your photo library.
- **Add to Photos** (`NSPhotoLibraryAddUsageDescription`): saving takes and captioned videos. Readglide asks only to add; it cannot see what is already in your library.

Before a recording starts, Readglide checks the free storage (disk-space API, reason E174.1), again only on the device.

## Stage 3: reviewing a take

**Speech Recognition** (`NSSpeechRecognitionUsageDescription`) is asked for the first time you open a take's review, which is where scoring and script captions are made. Readglide turns the take's audio into text **on the device only** and lines it up with your script. If the device has no on-device recognizer for the script's language, Readglide does not recognize the take at all; audio is never sent to the developer, to Apple's servers or to any third party. The recognized words are thrown away when the review screen closes; they are not saved.

To make scoring and captions possible, Readglide holds working copies in its on-device cache:

- **Your latest video take**: one copy, removed when you close the recording screen, start the next take, a recording is interrupted, or Readglide is next launched.
- **Your latest audio-only practice recording**: one copy (it never goes to Photos), removed when you close the review screen, start the next recording, close the practice panel, close the recording screen, or Readglide is next launched.
- **While the review screen is open**: one further copy of the take under review, video or audio, removed when that screen closes (or at the next launch).

What stays after a review is **numbers only**, saved per script as a practice history so you can follow your progress: when the take was scored, the read-as-written rate, lines read and the script's line count, skipped lines, speaking rate, how many long pauses there were, spoken time, and target time. Each take is tagged with a code that connects to nothing else (it cannot be used to find the video in your photo library); it exists only so one take is not counted twice. The history never holds the script's text, the recognized words, audio or video, and it never leaves the device. Each script keeps its latest 100 takes, and deleting the script deletes its history. A script you only pasted and read without saving loses its history at the next launch.

## Stage 4: exporting and sharing

A captioned video is added to Photos (add-only, as above). Once a video or subtitle file is out of Readglide, where it goes next is your decision.

If you put a slate at the start of a captioned video (a card showing your name, the role, and your agency or contact details), what you type is kept only on the device, in Readglide's settings: the name and agency or contact details once, and the role per script. It appears only as text inside the videos you export with that slate and is never sent to the developer or anyone else. A script's role is deleted with the script, and the role of a script you did not save (one you only pasted and read) is deleted at the next launch.

## What Readglide never does

- It never connects to a network. No analytics service (Google Analytics, Firebase or similar), advertising SDK or crash-reporting service is built in.
- It has no account to sign in to. The only name it ever stores is one you choose to type on a slate (Stage 4), and that stays on the device.
- It never reads device identifiers or advertising IDs, never tracks you, keeps no usage logs and has no use for your location.
- It sends no crash reports. If crash reporting is ever added, that will be disclosed separately.

Readglide's privacy manifest (`PrivacyInfo.xcprivacy`) tells Apple "No Data Collected". The three required-reason APIs named above are the only ones it uses, and none of them serves tracking.

## Buying Readglide

Readglide is a paid app bought once on the App Store; there are no in-app purchases and no subscription. Apple completes the purchase at download and handles all billing; the developer never sees card numbers or any other payment details. Apple's own policy covers that part: https://www.apple.com/legal/privacy/

## Younger users

Readglide is rated 4+. Nothing is sold inside the app; when a child under 13 buys the app itself, Apple's parental tools (Family Sharing and Screen Time) are the recommended way for a parent to stay in control.

## Removing what Readglide stored

The developer holds none of your information, so there is nothing to disclose or erase on request. Everything Readglide stored is on your device, and you can remove it whenever you like by deleting a script, using Readglide's Settings screen, or deleting the app:

- scripts you wrote, pasted or imported
- preferences (text size, line spacing, colors and themes, scroll speed, mirroring, each script's target time, and so on)
- each script's practice history (removed with the script)
- the slate's name, agency or contact details, and per-script roles. With the slate switched on, clearing its fields on the review screen of a take that can be exported as a captioned video deletes them; clearing the role there deletes only the role of that take's script. The name and agency or contact details also go when the app is deleted, and a role goes when its script is deleted.

## Updates to this page

This page may change when the law changes or Readglide gains features. Important changes will be announced in the app or here.

## Contact

Questions about this policy or about how Readglide is run:

- **Developer**: Kohei Omori
- **Email**: [konpei.work@gmail.com](mailto:konpei.work@gmail.com)

---

[← Home](./)
