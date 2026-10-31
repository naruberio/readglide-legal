---
layout: default
title: Privacy Policy
permalink: /privacy
---

# Privacy Policy

**Last updated: October 31, 2026**

Readglide is a teleprompter for iPhone and iPad made by Kohei Omori, a sole proprietor based in Japan (called "the developer" below). This page walks through the app in the order you use it (writing a script, reading and recording, reviewing a take, exporting) and says at each stage what Readglide keeps, where, and when it goes away. None of it reaches the developer: Readglide has no server, no account and no network code, and it collects no personal information.

---

## Stage 1: writing a script

The scripts you type, paste or import, and your display and scrolling preferences, are written to Readglide's own storage on your iPhone or iPad. Readglide never uploads them, neither to the developer nor to any other company.

If you back up your device (to iCloud or to a computer), Readglide's scripts, practice history, Read-Aloud Log and settings, slate entries included, go into that backup like any other app's data (section takes and audiobook recordings do not; see Stages 2 and 3). The backup lives in the iCloud account or on the computer you chose; the developer never receives it.

Two of Apple's "required reason" APIs are used at this stage, both purely on the device: user defaults (reason CA92.1) hold your preferences, and file timestamps (reason C617.1) let the library list and re-index saved scripts.

## Stage 2: reading, recording and practicing aloud

Scrolling a script needs no permission at all. The optional features below ask iOS for their permissions one at a time, each with an explanation, the first time you use them; saying no switches off only that feature. Readglide never asks for location, contacts or notifications.

- **Camera** (`NSCameraUsageDescription`): filming while the script is on screen. The video is recorded on the device, and Readglide sends it nowhere.
- **Microphone** (`NSMicrophoneUsageDescription`): sound for a video, and practice with audio only. Sound is written only into that video or that practice recording and is not transmitted. Practice recordings, audiobook recordings included (Stage 3), are never added to your photo library.
- **Add to Photos** (`NSPhotoLibraryAddUsageDescription`): saving takes, captioned videos, videos joined from section takes and videos with retakes cut out. Readglide asks only to add; it cannot see what is already in your library.

Timer & Bell, which you use without a script, needs no permission. Readglide makes the bell sound itself and plays it; it does not use the microphone and records nothing. Its duration and bell settings are kept with your other preferences in Readglide's settings on the device.

While you film, the video is written to the iOS temporary folder and removed once it has been added to Photos. If adding to Photos is not allowed, the file is left in place and goes when iOS clears its temporary folder.

A take recorded with Shoot by Section switched on is added to Photos as usual, and one copy is also kept in Readglide's own storage on the device, so you can pick a take for each heading and join them into one video. The copy stays even if adding to Photos is not allowed or fails. It stays until you delete it, or delete the script or Readglide (see "Removing what Readglide stored"). Because videos are large, these copies are kept out of device backups, so restoring a backup does not bring them back. Whatever was added to Photos stays in Photos.

Alongside each copy, Readglide keeps a small catalog entry: an ID for the take (a value that connects to nothing else, also used as the copy's file name), the section it covers (the heading's name, its position in the script, and which of the headings with that name it is), when it was recorded, its length and file size, its video format (resolution, frame rate, orientation, codec) and audio format (channel count, sample rate), whether it reached Photos, whether you picked it, and a short code computed from the section's text. The code is used only to tell whether the script changed after the take was recorded or scored. The catalog is kept with the copies and is also left out of device backups.

Before a recording starts, before a line retake in Audiobook Recordings starts, before section takes are joined, and before audiobook chapters are exported, Readglide checks there is enough free storage (disk-space API, reason E174.1), and the Section Takes list shows you the free storage (the same API, reason 85F4.1). Both happen only on the device.

## Stage 3: reviewing a take

**Speech Recognition** (`NSSpeechRecognitionUsageDescription`) is requested the first time you open the review of a take, the Section Takes list while it has a take not yet scored, or the Audiobook Recordings list while its latest recording has not been checked against the script, when the device can recognize the script's language. Scoring and script captions are made on the review screen; section takes are scored in their list, and audiobook recordings are checked in theirs. Readglide turns the take's audio into text **on the device only** and lines it up with your script. If the device has no on-device recognizer for the script's language, Readglide does not recognize the take at all; audio is never sent to the developer, to Apple's servers or to any third party. The recognized words are thrown away when the review screen closes; they are not saved.

The review screen also shows Fillers and off-script words for every take except a read-aloud reading, and, for the Announcement or news reading and Narration samples opened from "What are you practicing?" in the script list, a Target pace or a Time slot. All of these are worked out on the device from the same recognized words and are not saved, not even in the practice history. The one thing kept is the time slot you pick for the Narration sample, which is stored with your preferences.

To make scoring and captions possible, Readglide holds working files in its on-device cache:

- **Your latest video take** (except takes recorded with Shoot by Section): one copy, removed when you close the recording screen, start the next take, a recording is interrupted, or Readglide is next launched.
- **Your latest audio-only practice recording**: the recording itself (it never goes to Photos), removed when you close the review screen, start the next recording, close the practice panel, close the recording screen, or Readglide is next launched. If Keep in Recordings is on when the recording ends (you stop it, Readglide goes to the background, or a call stops it), a copy is kept as an audiobook recording first (see below).
- **While the review screen is open**: one further copy of the take under review, video or audio, removed when that screen closes (or at the next launch).

Except when you add a reading to the Read-Aloud Log (next paragraph), what stays after a review is **numbers only**, saved per script as a practice history so you can follow your progress: when the take was scored, the read-as-written rate, lines read and the script's line count, skipped lines, speaking rate, how many long pauses there were, spoken time, and target time. Each take is tagged with a code that connects to nothing else (it cannot be used to find the video in your photo library); it exists only so one take is not counted twice. The history never holds the script's text, the recognized words, audio or video, and Readglide never sends it off the device. Each script keeps its latest 100 takes, and deleting the script deletes its history. A script you only pasted and read without saving, and the sample scripts opened from "What are you practicing?" in the script list (they are never saved), lose their history at the next launch.

For a take read aloud from Read-Aloud Log in the script list, Readglide adds one entry to the log only when you tap "Add to log" on the review screen (nothing is kept if you don't). The entry holds when you read, the script's title (up to 80 characters), the reading time, the read-as-written rate, lines read and the script's line count, how many spots to practice there were together with **the script's text** for the first 20 of them (the spot itself and a few characters on each side), whether a grown-up listened, and the same take code as the practice history (used only so one take is not logged twice). The script's text is kept so you can look back at where the reading went wrong and hand the log to a teacher. Audio, video and the recognized words are never in it, and spots to practice can include recognition errors. The log is kept in Readglide's own storage on the device, separately from your scripts: deleting a script does not delete it (it is a record of homework done), and it keeps the latest 2,000 readings. Readglide never sends the log off the device.

When you open the Section Takes list, any section take not yet scored is scored the same way, on the device only, and the recognized words are not kept. What stays is a few numbers added to that take's catalog entry from Stage 2 (the read-as-written rate, lines read and the section's line count, skipped lines, or a mark if the take could not be scored), the section's code at the time of scoring, and where to trim the start and end when joining (in seconds). These scores do not go into the practice history.

**Audiobook recordings.** In Practice with audio only, a switch called Keep in Recordings keeps the recording inside Readglide instead of letting it go after the review. It starts on for the Audiobook reading sample and for a script that already has recordings; for other saved scripts and the other samples you turn it on yourself, and it is not offered for a script you only pasted and read. A recording is kept when you stop it, when Readglide goes to the background, or when a call or another interruption stops it (what was recorded up to then). A recording stopped by closing the practice panel or the recording screen is not kept.

Each kept recording is one audio file (.m4a) in Readglide's own storage on the device (Application Support, in a folder named AudiobookTakes with one folder per script). It is never added to Photos and is left out of device backups, so restoring a backup does not bring it back. Next to the files Readglide keeps a small index, also left out of backups: an ID for each recording (a value that connects to nothing else, also used as the file name), when it was recorded, its length and, once the recording has been checked, a short code computed from the script's text (used only to tell whether the script changed since), the times at which each line and spoken heading start and end, which lines were misread or skipped, and, for each retake, its line, the script's code at that time, when it was recorded, which part of the recording it replaces, which part of the retake is used and whether the line was read as written. The recognized words and the script's text are not in it.

When you open Audiobook Recordings, the latest recording is checked against the script on the device only, in the same way as a take review, and the recognized words are thrown away when the check finishes. Retake records a single line: the retake is written to Readglide's on-device cache, checked against that line only, and then copied next to the recording; the cached file is removed once it has been copied, when you cancel or start another retake, when the retake recording is interrupted, when you close the list, or at the next launch. The original recording is never rewritten. Undo Retake deletes the retake's file, a new retake of the same line replaces the earlier one, and retakes recorded before the script was edited are deleted when the recording is checked again.

Audiobook recordings stay until you delete them in the list (a recording goes together with its retakes), delete the script, or delete Readglide. Recordings made with a sample script, which is never saved, are removed the next time Readglide is launched, and at each launch Readglide also removes recording files that are no longer in a saved script's index. For this it reads the folders' creation times, and for the list it reads the files' sizes, both on the device only (file timestamps and other file metadata, the same reason C617.1 as in Stage 1). Readglide never sends recordings off the device.

## Stage 4: exporting and sharing

A captioned video, a video joined from section takes or a video with retakes cut out is added to Photos (add-only, as above). A subtitle file, a month's image from the Read-Aloud Log, or the audio files exported from Audiobook Recordings go wherever you pick in the share sheet. Once a video, subtitle file, image or audio file is out of Readglide, where it goes next is your decision.

Exporting also puts files in the iOS temporary folder:

- **A captioned video while it is being made**: one file, removed as soon as it has been added to Photos (or as soon as the export fails or is cancelled).
- **The subtitle file (.srt)**: one file, made when scoring finishes so it is ready to share, and removed when the review screen closes.
- **A video being joined from section takes, or one being made with retakes cut out**: one file each, removed as soon as it has been added to Photos (or as soon as joining or cutting fails or is cancelled, or adding it to Photos is not allowed or fails).
- **Silent audio files**: made to fill the parts of a take where its sound is shorter than its video, and removed once joining or cutting finishes, fails or is cancelled.
- **A month's image from the Read-Aloud Log (PNG)**: one file, made on the Read-Aloud Log screen when the month shown has entries, so it is ready for "Share this month". It shows each entry's date, script title, reading time, the number of spots to practice with the script's text for the first 3 of them, and whether a grown-up listened, plus the month's count and total time. It is removed when it is remade for another month or changed entries, and when the Read-Aloud Log screen closes.

If Readglide quits partway and leaves any of these behind, it goes when iOS clears its temporary folder.

Export by Chapter in Audiobook Recordings writes one audio file (AAC, .m4a) per heading, or a single file, to Readglide's on-device cache, each named with a number and the heading's text ("Opening" for the part before the first heading, or the script's title when everything goes into one file), so that Share Exported Files can hand them over. These files are removed at the next export, when you close Audiobook Recordings, or at the next launch. Files you have already shared stay wherever you sent them.

If you put a slate at the start of a captioned video (a card showing your name, the role, and your agency or contact details), what you type is kept only on the device, in Readglide's settings: the name and agency or contact details once, and the role per script. It appears only as text inside the videos you export with that slate, and Readglide never sends it to the developer or anyone else. A script's role is deleted with the script, and the role of a script you did not save (one you only pasted and read, or a sample from "What are you practicing?") is deleted at the next launch.

## What Readglide never does

- It never connects to a network. No analytics service (Google Analytics, Firebase or similar) or advertising SDK is built in.
- It has no account to sign in to. The only name it ever stores is one you choose to type on a slate (Stage 4), and Readglide never sends that off the device.
- It never reads device identifiers or advertising IDs, never tracks you, keeps no usage logs and has no use for your location.
- No crash-reporting service is built in, and it sends no crash reports. If crash reporting is ever added, that will be disclosed separately.

Readglide's privacy manifest (`PrivacyInfo.xcprivacy`) tells Apple "No Data Collected". The three required-reason APIs named above are the only ones it uses, and none of them serves tracking.

## Buying Readglide

Readglide is a paid app bought once on the App Store; there are no in-app purchases and no subscription. Apple completes the purchase at download and handles all billing; the developer never sees card numbers or any other payment details. Apple's own policy covers that part: https://www.apple.com/legal/privacy/

## Rating request

When you close the review screen of a take that beat your personal best, Readglide may ask iOS to show its rating prompt (at most once per app version; iOS decides whether it actually appears and how often). The prompt belongs to Apple: any rating or review you leave goes to Apple and is handled under Apple's privacy policy. Readglide is never told whether you rated it or what you wrote (reviews published on the App Store can be read by the developer, as by anyone else). All Readglide keeps is the app version number at which it asked.

## Younger users

Readglide is rated 4+. Nothing is sold inside the app; when a child under 13 buys the app itself, Apple's parental tools (Family Sharing and Screen Time) are the recommended way for a parent to stay in control.

Read-Aloud Log in the script list is for a parent who listens to a child reading aloud and keeps a record of it (what it keeps is in Stage 3). The recording is handled on the device only, as with practice with audio only, and the log never reaches the developer either. If the reading uses a saved script with Keep in Recordings on (it starts on for a script that already has audiobook recordings), that recording is also kept as an audiobook recording (Stage 3) until it is deleted.

## Removing what Readglide stored

The developer holds none of your information, so there is nothing to disclose or erase on request. Everything Readglide stored is on your device (for device backups, see the end of this section), and you can remove it whenever you like by deleting a script, using Readglide's Settings screen, the Section Takes list, the Audiobook Recordings list or the Read-Aloud Log screen, or deleting the app:

- scripts you wrote, pasted or imported
- preferences (text size, line spacing, colors and themes, scroll speed, mirroring, each script's target time, the Narration sample's time slot, the Timer & Bell duration and bell settings, and so on)
- the app version number at which Readglide asked for a rating (removed when the app is deleted)
- each script's practice history (removed with the script)
- the Read-Aloud Log. On the Read-Aloud Log screen you can delete one reading at a time (tap it and choose Delete, or swipe it left). It is not removed when a script is deleted; it goes when the app is deleted. If the log's file ever becomes unreadable (for example, because it is damaged), Readglide keeps that file on the device under another name instead of overwriting it, and starts a new log; that file also goes when the app is deleted.
- the slate's name, agency or contact details, and per-script roles. With the slate switched on, clearing its fields on the review screen of a take that can be exported as a captioned video deletes them; clearing the role there deletes only the role of that take's script. The name and agency or contact details also go when the app is deleted, and a role goes when its script is deleted.
- copies of section takes and their catalog entries. In the Section Takes list you can delete one take, a section's takes, the takes you did not pick after joining, or all of a script's takes. They also go when the script or the app is deleted. Copies added to Photos stay there; delete them in the Photos app.
- audiobook recordings, their retakes and their index. In Audiobook Recordings you can delete one recording at a time, together with its retakes. They also go when the script or the app is deleted, and those made with a sample script go at the next launch. Audio files you exported and shared stay where you sent them.

Whatever went into a device backup stays in that backup. For iCloud Backup, switching Readglide off in the list of apps to back up, in iOS Settings, and confirming the deletion removes just Readglide's part. A backup on a computer cannot have Readglide's part removed on its own; clearing it there means deleting that whole backup, other apps' data included.

## Updates to this page

This page may change when the law changes or Readglide gains features. Important changes will be announced in the app or here.

## Contact

Questions about this policy or about how Readglide is run:

- **Developer**: Kohei Omori
- **Email**: [konpei.work@gmail.com](mailto:konpei.work@gmail.com)

---

[← Home](./)
