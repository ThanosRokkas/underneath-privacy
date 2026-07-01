---
layout: default
title: Privacy Policy
---

# Privacy Policy

**Effective Date:** June 28, 2026
**Last Updated:** June 28, 2026

Underneath ("we," "our," or "the App") is a food label scanning application that helps users understand what is in the products they buy. This Privacy Policy explains how we collect, use, store, and protect your information.

**Contact:** [thanosrokkas@gmail.com](mailto:thanosrokkas@gmail.com)
**Website:** [underneath.app](https://underneath.app)

---

## 1. Information We Collect

### 1.1 Account Information

When you create an account, we collect:

- **Email address** — provided during sign-up or via Apple/Google Sign-In
- **Display name** — derived from your sign-in provider or email address
- **Authentication tokens** — used to verify your identity (not stored by us directly; managed by Supabase Auth)

### 1.2 Health & Diet Preferences

During onboarding, you may optionally provide:

- Health goals (e.g., lose weight, eat cleaner)
- Dietary preferences (e.g., vegan, keto)
- Allergy information (e.g., gluten, dairy)
- Additives you want to avoid
- Ultra-processed food flagging preference
- Reading habits

These preferences are stored **locally on your device** using AsyncStorage and, when you are signed in, **synced to your profile on our servers** so they persist across devices.

### 1.3 Scan History

When you scan a product barcode, we store:

- Barcode number
- Product name and brand
- Health score and rating level
- Product image URL (from Open Food Facts)
- Timestamp of the scan
- A randomly generated device identifier (not your hardware ID)
- Your user ID (if you are signed in)

### 1.4 Subscription Information

If you subscribe to Underneath Plus, we store:

- Subscription status and product ID
- Current billing period dates
- Store (Apple App Store or Google Play)
- RevenueCat customer ID

### 1.5 Referral Information

If you participate in our referral program, we store:

- Your unique referral code (auto-generated)
- Referral relationships (inviter and invitee IDs)
- Referral status

### 1.6 Country Code

We detect your country to tailor regulatory information (e.g., EU vs. FDA additive status). This is stored locally on your device.

---

## 2. Information We Do NOT Collect

- **No camera images are transmitted.** The camera is used exclusively for barcode scanning on your device. No photos or images are sent to our servers.
- **No analytics or tracking.** We do not use Firebase Analytics, Sentry, Amplitude, Mixpanel, or any other analytics or crash-reporting SDK.
- **No advertising.** The App contains no ads and no advertising SDKs.
- **No cookies.** As a mobile application, we do not use cookies or web tracking technologies.
- **No location data.** We do not access or store your precise location.
- **No contacts, microphone, or other sensitive permissions.**

---

## 3. How We Use Your Information

We use the information we collect to:

- Provide and improve the food scanning and scoring service
- Display your scan history
- Manage your subscription and trial period
- Facilitate the referral program
- Show regulatory information relevant to your country

---

## 4. Third-Party Services

We use a limited number of third-party services, each for a specific purpose:

### 4.1 Supabase

- **Purpose:** Database hosting, user authentication, and serverless functions
- **Data shared:** Account information, scan history, subscription and referral records
- **Privacy policy:** [https://supabase.com/privacy](https://supabase.com/privacy)

### 4.2 RevenueCat

- **Purpose:** Subscription and in-app purchase management
- **Data shared:** User ID and purchase/subscription information
- **Privacy policy:** [https://www.revenuecat.com/privacy](https://www.revenuecat.com/privacy)

### 4.3 Open Food Facts

- **Purpose:** Product data lookup (name, ingredients, nutrition facts, images)
- **Data shared:** Barcode number only (public API, no user data sent)
- **Privacy policy:** [https://world.openfoodfacts.org/privacy](https://world.openfoodfacts.org/privacy)

### 4.4 Apple Sign-In / Google Sign-In

- **Purpose:** Authentication
- **Data shared:** We receive an identity token from Apple or Google to verify your account. We do not access your Apple ID password or Google account password.

We do **not** sell, rent, or share your personal data with any other third parties.

---

## 5. Data Storage & Security

### 5.1 Server-Side Storage

Your account data, scan history, and subscription information are stored in a PostgreSQL database hosted by Supabase Cloud. We protect this data with:

- **Row Level Security (RLS):** Database policies ensure users can only access their own data
- **Service-role separation:** Sensitive operations (subscription updates, product ingestion) run through authenticated serverless functions
- **Rate limiting:** API endpoints are rate-limited to prevent abuse

### 5.2 On-Device Storage

- **AsyncStorage:** Health preferences, onboarding state, and recent searches are stored locally on your device in unencrypted app-sandboxed storage
- **SecureStore (Expo):** Authentication tokens are stored in your device's secure keychain/keystore (encrypted by the operating system)

### 5.3 Data Transmission

All data transmitted between the App and our servers uses HTTPS/TLS encryption.

---

## 6. Data Retention & Deletion

### 6.1 Retention

- Account data is retained as long as your account is active
- Scan history is retained as long as your account exists or the device ID is associated with scan records
- Cached product data (not personal) may be retained indefinitely to improve service performance

### 6.2 Account Deletion

You can delete your account directly within the App by going to your profile and tapping "Delete account." You may also request deletion by contacting us at [thanosrokkas@gmail.com](mailto:thanosrokkas@gmail.com).

When your account is deleted:

- Your profile, subscription, and referral records are **permanently deleted** (cascading delete)
- Scan history associated with your user ID is removed
- Local data on your device can be cleared by uninstalling the App

In-app deletion is processed immediately. Email requests will be processed within 30 days.

---

## 7. Your Rights

Regardless of where you are located, you have the right to:

- **Access** your personal data
- **Correct** inaccurate information
- **Delete** your account and data
- **Export** your data in a portable format
- **Object** to processing of your data
- **Withdraw consent** at any time

These rights are aligned with GDPR (EU), CCPA (California), and other applicable privacy regulations. To exercise any of these rights, contact us at [thanosrokkas@gmail.com](mailto:thanosrokkas@gmail.com).

---

## 8. Children's Privacy

Underneath is not directed at children under the age of 13. We do not knowingly collect personal information from children under 13. If we become aware that we have collected data from a child under 13, we will promptly delete that information. If you believe a child under 13 has provided us with personal data, please contact us at [thanosrokkas@gmail.com](mailto:thanosrokkas@gmail.com).

---

## 9. Health Disclaimer

The health scores, ingredient analysis, and additive information provided by Underneath are for **informational purposes only**. They do not constitute medical advice, dietary guidance, or a substitute for professional health consultation. Always consult a qualified healthcare provider for dietary or medical decisions.

---

## 10. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the "Last Updated" date at the top of this page. We encourage you to review this policy periodically. Continued use of the App after changes constitutes acceptance of the updated policy.

---

## 11. Contact Us

If you have any questions or concerns about this Privacy Policy or our data practices, please contact us at:

**Email:** [thanosrokkas@gmail.com](mailto:thanosrokkas@gmail.com)
**Website:** [underneath.app](https://underneath.app)
