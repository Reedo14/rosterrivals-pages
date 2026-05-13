---
title: Privacy Policy
---

# Roster Rivals — Privacy Policy

**Effective date:** May 10, 2026

This policy explains what data Roster Rivals collects, how we use it, and what we don't do. It applies to the Roster Rivals iOS app and any future Android or web versions.

We try to be honest and minimal. The shorter version: we collect what's needed to sign you in, deliver push notifications, serve non-personalized ads, and run gameplay analytics. We don't sell your data. We don't run third-party analytics SDKs. We don't track you across other apps.

If anything below is unclear, email us at the address at the bottom of this page.

---

## 1. What we collect

### Account & profile

When you sign up, we collect:

- **Email address** — used to sign you in and to email you about your account
- **Username** — visible to other players
- **Phone number** (10-digit, normalized) — used to find friends already on Roster Rivals when you grant Contacts permission. Never displayed to other players
- **Password** — stored as a salted hash by our auth provider (Supabase). We never see or store your plaintext password

During onboarding you can optionally tell us:

- **Favorite NFL team, favorite NBA team, home state, year of birth** — used to tailor gameplay analytics and to help us improve the trivia experience. Optional. Not visible to other players

### Push notifications

If you grant notification permission, we store an **Expo push notification token** on your account so we can deliver:

- Friend requests
- Game invites
- Direct challenges
- Clan messages
- Weekly challenge reminders

You can disable any of these categories in Settings. The token itself never leaves our servers and is never shared with other players.

### Gameplay data

When you play a match, we record:

- Each chain answer you submit (the player name and team you typed)
- How long you took to answer (in seconds)
- The match outcome (rank, points earned, win/loss)
- The category each answer matched on (team / jersey / college / direct)

This data lives in a `submissions` table and is used to balance the game (timer tuning, difficulty curves, validator improvements). Your username appears on public leaderboards and in completed game histories visible to your opponents in that match.

### Advertising

Roster Rivals uses **Google AdMob** to serve banner and interstitial ads. We have configured AdMob to request **non-personalized ads only**, which means ads are based on the broad context of the app rather than your personal browsing history.

Even with non-personalized ads, AdMob still receives:

- Your device's advertising identifier (IDFA on iOS)
- Your IP address
- Your country/region
- Device type, operating system, and screen size
- The app version

This is unavoidable for any app showing ads. AdMob's own privacy policy is at https://policies.google.com/privacy.

### Contacts (only if you grant permission)

If you tap "Find friends" and grant Contacts permission, we read the names and phone numbers from your device address book to check which of your contacts already have Roster Rivals accounts.

- **Numbers that match an existing player:** the match is shown in the friends-finder list. Nothing else happens.
- **Numbers that do not match:** they stay on your device. We do not upload them. We do not store them. We do not use them later.

You can revoke Contacts permission at any time in iOS Settings.

### Local data on your device

The app stores a few small things in your device's local storage that never leave the device:

- Your last sign-in email (for convenience on the login screen)
- Your notification preferences
- Your tutorial completion flags
- Your solo best score
- Cached game state and recent gameplay picks

This data is wiped when you delete the app.

---

## 2. What we don't do

- **No third-party analytics SDKs.** We do not use Sentry, PostHog, Mixpanel, Amplitude, Firebase Analytics, Segment, or any similar service. Our gameplay analytics live in our own database
- **No personalized advertising.** We have set `requestNonPersonalizedAdsOnly: true` for every ad request
- **No upload of non-matching contacts.** Contacts that don't already have a Roster Rivals account stay on your device
- **No sale of your personal data**
- **No cross-app tracking.** We do not show the iOS App Tracking Transparency prompt because we do not track you across other apps and websites
- **No data collected for children.** Roster Rivals is not directed at children under 13

---

## 3. Where your data goes

| Service | What they receive | Why |
|---|---|---|
| Supabase (US region) | Account, profile, gameplay, friends, clans, push tokens | Backend storage |
| Google AdMob | IDFA, IP, country, device type, app version | Non-personalized ad delivery |
| Apple Push Notification Service / Google FCM (via Expo) | Your push token + the text of the notification | Notification delivery |

We do not share data with any other third parties.

---

## 4. What other players can see

Some data is intentionally public on Roster Rivals so the social parts of the game work:

- **Visible to anyone:** your username, current rank, total points, win count, current streak
- **Visible to your friends:** your friendship status (pending / accepted)
- **Visible to clan members:** any messages you send in clan chat
- **Visible only to you and our backend:** your email, phone number, password, push token, year of birth, favorite teams, home state

When you share your friend code (RR-XXXX), anyone with that code can send you a friend request.

---

## 5. Children's data

Roster Rivals is not directed at children under the age of 13, and we do not knowingly collect data from children under 13. If you believe a child under 13 has created an account, please email us and we will delete the account.

---

## 6. Your rights

You can:

- **Delete your account.** Use the "Delete account" option in Settings, or email us. Account deletion removes your profile, friend graph, push token, and submissions
- **Export your data.** Email us and we will send you the data we hold for your account
- **Revoke permissions.** Notifications and Contacts permissions can be revoked at any time in iOS Settings → Roster Rivals
- **Ask a question.** Email us at the address below

---

## 7. Security

Passwords are hashed by our auth provider; we never see them. Data is transmitted to our backend over TLS. Account-level data is protected by row-level security policies in our database, meaning even our own backend code can only read data on behalf of an authenticated user.

No system is perfectly secure. If we discover a breach affecting your account, we will notify you by email.

---

## 8. Changes to this policy

If we change how we collect or use your data — for example, if a future version of Roster Rivals adds a new feature that collects new information — we will update this page and update the "Effective date" at the top. Material changes will also be communicated in-app or by email.

---

## 9. Contact us

For privacy questions, account deletion, or data export requests:

**rosterrivals@gmail.com**

We aim to respond within 7 days.

---

[← Back to main](index.html)
