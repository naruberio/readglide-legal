---
layout: default
title: Privacy Policy
permalink: /privacy
---

# Privacy Policy

**Last updated: September 28, 2026**

Kohei Omori (a sole proprietor, hereinafter the "Operator", "we", "us", or "our") provides this Privacy Policy to explain how we handle your information in the iOS application "**Readglide**" (a teleprompter, the "App").

---

## 1. Core principle

The App works **entirely on your device**. The scripts you write or paste, and all display and scroll settings, are stored only on your device and are never transmitted to our servers or any third-party servers. We do **not collect personal information** through the App.

## 2. Information we collect

The App does not collect any personal information, as detailed below.

| Information category | Collected? | Reason |
|---------------------|:---------:|--------|
| Name, email, contact info | ✗ Not collected | No account features (a name or contact entered for a slate stays on your device; see §3) |
| Your scripts / text | ✗ Not collected | Stored on-device only, no external transmission |
| Location data | ✗ Not collected | Not required by functionality |
| Device identifiers, advertising IDs | ✗ Not collected | No tracking |
| Usage history, operation logs | ✗ Not collected | No analytics |
| Crash reports | ✗ Not collected | Not integrated (any future adoption will be separately disclosed) |

We declare "No Data Collected" in the App Privacy Manifest (`PrivacyInfo.xcprivacy`) to Apple. The only Apple "Required Reason" APIs the App uses are user-defaults access (reason code CA92.1) to store your settings, disk-space access (reason code E174.1) to check free storage before recording, and file-timestamp access (reason code C617.1) to list and re-index your saved scripts. All three are strictly on-device and unrelated to tracking.

## 3. Permissions used on device

Reading a script requires **no special permissions**. The optional features below ask for a permission, with an in-context explanation, the first time you use them. If you decline, everything else keeps working. The App never requests access to your location, contacts, or notifications.

| Permission | Feature | How it is handled |
|-----------|---------|-------------------|
| Camera (`NSCameraUsageDescription`) | Recording while the script is shown | Video is recorded on your device and never transmitted |
| Microphone (`NSMicrophoneUsageDescription`) | Recording audio with the video; practicing with audio only | Audio is written only to the recording or the practice recording and never transmitted. Practice recordings are not saved to your photo library |
| Add to Photos (`NSPhotoLibraryAddUsageDescription`) | Saving recordings and captioned videos | Add-only access; the App never reads your photo library |
| Speech Recognition (`NSSpeechRecognitionUsageDescription`) | Scoring a video or audio take and script captions | The recording's audio is transcribed **on your device only** and matched to your script. If your device cannot recognize the language on-device, no recognition is performed; audio is never sent to our servers, Apple's servers, or any third party. Recognition results are discarded when you close the review screen and are not stored |

For scoring and captions, a copy of your most recent take is kept in the App's on-device cache. It is deleted when you close the recording screen, start the next take, when a recording is interrupted, or the next time you launch the App. While the review screen is open, it keeps one more copy for itself, which is deleted when you close the review screen (or the next time you launch the App).

When you practice with audio only (recording with the microphone, without the camera), the recording is not saved to your photo library; only the most recent one is kept in the App's on-device cache. It is deleted when you close the review screen, start the next recording, close the practice panel, close the recording screen, or the next time you launch the App. While the review screen is open, it keeps one more copy for itself, as with videos, which is deleted when you close the review screen (or the next time you launch the App).

**Only the numbers** from each score (when it was scored, the read-as-written rate, lines read and the script's line count, skipped lines, speaking rate, number of long pauses, spoken time, and target time) are kept on your device as a per-script practice history, used to show how your score changes. Each take also gets a code that is not linked to any other information (the code itself cannot be traced to the video in your photo library), only so the same take is not counted twice. The history never includes your script's text, the recognized words, audio, or video, and it is never transmitted. Up to the latest 100 takes are kept per script, and they are deleted together with the script. The history of a script you did not save (one you only pasted and read) is deleted the next time you launch the App.

If you use a slate (a card with your name, role, and agency or contact details at the start of a captioned video), the name and agency or contact details you enter, and the role you enter for each script, are stored only on your device (in the App's settings). They only appear as text in the videos you export with the slate and are never sent to us or any third party. Whether to share those videos is up to you. The role for a script is deleted together with the script, and the role for a script you did not save (one you only pasted and read) is deleted the next time you launch the App.

## 4. Communication with third parties

The App **does not communicate over the network at all**.

No third-party analytics services (Google Analytics, Firebase, etc.), advertising SDKs, or crash-reporting services are integrated into the App.

## 5. In-App Purchases

The App is a **paid app** and offers **no in-app purchases whatsoever**. There are no subscriptions either. The purchase completes at download time on the App Store; billing and payment information are handled **directly by Apple**, and we cannot access payment details (credit-card numbers, etc.).

For more information, please refer to Apple's Privacy Policy (https://www.apple.com/legal/privacy/).

## 6. Children's use

The App is rated 4+. There are no in-app purchases, but for the purchase of the App itself by children under 13, we recommend parents use Apple ID parental controls (Family Sharing, Screen Time) to manage usage.

## 7. Your rights

Since the App does not collect your information, we do not hold any data subject to disclosure or deletion requests.

The following information stored on your device can be deleted by you at any time — by deleting individual scripts, using the App's "Settings" screen, or removing the App:

- Scripts you have written or pasted
- App settings (font size, line spacing, colors / themes, scroll speed, mirror mode, per-script target time, etc.)
- Per-script practice history (the numbers from each score; deleted together with the script)
- The name, agency or contact details, and per-script role entered for the slate (deleted when you turn on the slate and clear the fields on the review screen of a take that can be exported as a captioned video, though clearing the role deletes only the role for that take's script; the name and agency or contact details are also deleted when you remove the App, and the role when you delete the script)

## 8. Changes to this Policy

This Policy may be revised due to legal changes or feature updates to the App. Significant changes will be notified within the App or on this page.

## 9. Contact

For inquiries regarding this Policy or how the App is operated, please contact:

- **Entity**: Kohei Omori
- **Email**: [konpei.work@gmail.com](mailto:konpei.work@gmail.com)

---

[← Home](./)
