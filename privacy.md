---
layout: default
title: Privacy Policy
permalink: /privacy
---

# Privacy Policy

**Last updated: August 9, 2026**

Kohei Omori (a sole proprietor, hereinafter the "Operator", "we", "us", or "our") provides this Privacy Policy to explain how we handle your information in the iOS application "**Readglide**" (a teleprompter, the "App").

---

## 1. Core principle

The App works **entirely on your device**. The scripts you write or paste, and all display and scroll settings, are stored only on your device and are never transmitted to our servers or any third-party servers. We do **not collect personal information** through the App.

## 2. Information we collect

The App does not collect any personal information, as detailed below.

| Information category | Collected? | Reason |
|---------------------|:---------:|--------|
| Name, email, contact info | ✗ Not collected | No account features |
| Your scripts / text | ✗ Not collected | Stored on-device only, no external transmission |
| Location data | ✗ Not collected | Not required by functionality |
| Device identifiers, advertising IDs | ✗ Not collected | No tracking |
| Usage history, operation logs | ✗ Not collected | No analytics |
| Crash reports | ✗ Not collected | Not integrated (any future adoption will be separately disclosed) |

We declare "No Data Collected" in the App Privacy Manifest (`PrivacyInfo.xcprivacy`) to Apple. The only Apple "Required Reason" APIs the App uses are user-defaults access (reason code CA92.1) to store your settings and file-timestamp access (reason code C617.1) to list and re-index your saved scripts. Both are strictly on-device and unrelated to tracking.

## 3. Permissions used on device

The current version (a pure text teleprompter) requires **no special permissions** — it does not request access to your camera, microphone, photos, location, contacts, or notifications.

*(Forward note)* If a future optional camera-overlay recording feature is released, it will request camera, microphone, and "Add to Photos" access, each with a separate, in-context explanation shown at the moment of use (`NSCameraUsageDescription` / `NSMicrophoneUsageDescription` / `NSPhotoLibraryAddUsageDescription`). The current version does not include this feature.

## 4. Communication with third parties

The App does not communicate over the network **except** for the following.

| Recipient | Purpose | Information transmitted |
|-----------|---------|------------------------|
| Apple StoreKit / App Store servers | In-app purchase (one-time only) | Billing information managed automatically by Apple. We do not access this information. |

No third-party analytics services (Google Analytics, Firebase, etc.), advertising SDKs, or crash-reporting services are integrated into the App.

## 5. In-App Purchases

The App offers a one-time "Readglide Pro" unlock through Apple's App Store In-App Purchase (IAP) feature. Billing and payment information are handled **directly by Apple**, and we cannot access payment details (credit-card numbers, etc.). There are **no subscriptions**.

For more information, please refer to Apple's Privacy Policy (https://www.apple.com/legal/privacy/).

## 6. Children's use

The App is rated 4+, but for in-app purchases by children under 13, we recommend parents use Apple ID parental controls (Family Sharing, Screen Time) to manage usage.

## 7. Your rights

Since the App does not collect your information, we do not hold any data subject to disclosure or deletion requests.

The following information stored on your device can be deleted by you at any time — by deleting individual scripts, using the App's "Settings" screen, or removing the App:

- Scripts you have written or pasted
- App settings (font size, line spacing, colors / themes, scroll speed, mirror mode, etc.)
- The free-tier saved-script count

## 8. Changes to this Policy

This Policy may be revised due to legal changes or feature updates to the App. Significant changes will be notified within the App or on this page.

## 9. Contact

For inquiries regarding this Policy or how the App is operated, please contact:

- **Entity**: Kohei Omori
- **Email**: [konpei.work@gmail.com](mailto:konpei.work@gmail.com)

---

[← Home](./)
