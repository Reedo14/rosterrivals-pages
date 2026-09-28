---
title: Privacy Policy
---

# Roster Rivals Privacy Policy

**Effective date:** September 28, 2026

This policy explains what data Roster Rivals collects, how we use it, and what we don't do. It applies to the Roster Rivals iOS app and any future Android or web versions.

We try to be honest and minimal. The shorter version: we collect what's needed to sign you in, deliver push notifications, serve non-personalized ads, run gameplay analytics, and understand what kinds of sports fans play. We don't sell your personal data. We don't run third-party analytics SDKs. We don't track you across other apps.

If anything below is unclear, email us at the address at the bottom of this page.

---

## 1. What we collect

### Account & profile

When you sign up, we collect:

- **Email address**: used to sign you in and to email you about your account
- **Username**: visible to other players
- **Phone number** (10-digit, normalized): used to find friends already on Roster Rivals when you grant Contacts permission. Never displayed to other players
- **Password**: stored as a salted hash by our auth provider (Supabase). We never see or store your plaintext password

### Your fan profile

During onboarding we ask for a few things. You can change them anytime in Settings under "Your fan profile."

Required to play:

- **Your age range** (13-17, 18-24, 25-34, 35-44, 45+). We do not ask for or keep your birth date or birth year. If you told us your birth year in an earlier version of the app, we converted it to an age range and deleted the year.
- **Your favorite football team and favorite basketball team.** "No favorite" is a fine answer.

Optional:

- **Your ZIP code.** We keep only the first 3 digits (for example, 606 for 60614). Your full ZIP code never leaves your phone. We use the first 3 digits to place you in a broad metro area (a U.S. Census "CBSA") so we can understand where our fans are.
- **Your phone number**, so friends already on Roster Rivals can find you.

None of these are shown to other players.

### Push notifications

If you grant notification permission, we store an **Expo push notification token** on your account so we can deliver:

- Friend requests
- Game invites
- Direct challenges
- Clan messages
- Weekly challenge reminders

You can disable any of these categories in Settings. The token itself never leaves our servers and is never shared with other players.

### Gameplay data

When you play (multiplayer games, Solo, vs CPU and Daily Drill), we record:

- Each answer you give: whether it was right, which player, team, college or jersey number it was, the player or team you were linking from, how long you took, and the game mode. For wrong answers we keep what you typed so we can find and fix answers our checker got wrong.
- When you open and close the app (the start and end time of each session, the hour of day on your phone, and which game modes you played).
- The match outcome (rank, points earned, win or loss).

We use this to improve the game (answer checking, difficulty, timers) and to understand, in aggregate, what kinds of sports fans play Roster Rivals. This data stays in our own database. Your username appears on public leaderboards and in completed game histories visible to your opponents in that match.

### Marketing emails (only if you opt in)

If you check "Send me sports news, offers and giveaways from Roster Rivals, including from our partners," we may email you about those things. We record when you opted in or out and where (sign-up, the in-app prompt, or Settings). You can turn this off anytime in Settings. We never opt in anyone who told us they are under 18, and we turn it off automatically if you later tell us you are under 18. We do not give your email address to partners.

### Purchases

If you make an in-app purchase (like coins or Remove Ads), Apple processes the payment. We receive a record of the purchase (what you bought and when) through RevenueCat, the service that verifies in-app purchases, so we can credit your account. We never see your payment card details.

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

### How we use fan data

We may create aggregated, de-identified insights from gameplay and fan profile data, for example "fans aged 25-34 in the Chicago area know more 1980s players." These reports:

- never include your name, username, email, phone number or any individual's answers;
- never include anyone who told us they are 13-17;
- are only produced for groups large enough that no individual can be singled out.

We do not share individual-level data with sponsors, advertisers or data brokers. If that ever changed, we would ask for your explicit permission first.

---

## 2. What we don't do

- **No third-party analytics SDKs.** We do not use Sentry, PostHog, Mixpanel, Amplitude, Firebase Analytics, Segment, or any similar service. Our gameplay analytics live in our own database
- **No personalized advertising.** We have set `requestNonPersonalizedAdsOnly: true` for every ad request
- **No upload of non-matching contacts.** Contacts that don't already have a Roster Rivals account stay on your device
- **No sale of your personal data.** We do not sell your personal data
- **No cross-app tracking.** We do not show the iOS App Tracking Transparency prompt because we do not track you across other apps and websites
- **No accounts for children.** Roster Rivals is not for children under 13 (see section 5)

---

## 3. Where your data goes

| Service | What they receive | Why |
|---|---|---|
| Supabase (US region) | Account, profile, gameplay, friends, clans, push tokens | Backend storage |
| RevenueCat | Your account ID (a random code, not your name or email) and your purchase records | Verifying in-app purchases |
| Google AdMob | IDFA, IP, country, device type, app version | Non-personalized ad delivery |
| Apple Push Notification Service / Google FCM (via Expo) | Your push token + the text of the notification | Notification delivery |

We do not share data with any other third parties.

---

## 4. What other players can see

Some data is intentionally public on Roster Rivals so the social parts of the game work:

- **Visible to anyone:** your username, current rank, total points, win count, current streak
- **Visible to your friends:** your friendship status (pending / accepted)
- **Visible to clan members:** any messages you send in clan chat
- **Visible only to you and our backend:** your email, phone number, password, push token, favorite teams, ZIP area (first 3 digits), age range and marketing email choice

When you share your friend code (RR-XXXX), anyone with that code can send you a friend request.

---

## 5. Children's data

Roster Rivals is not for children under 13. When we ask for your age range, anyone who picks "Under 13" can't continue: their account is deleted right away and they are signed out. We don't keep that answer. If we learn in any other way that a child under 13 has given us personal information, we will delete it. Parents can contact us at rosterrivals@gmail.com.

Players aged 13-17 are never opted in to marketing emails and are never included in the aggregated fan insights described above.

---

## 6. Your rights

You can:

- **Delete your account.** Use the "Delete account" option in Settings, or email us. Account deletion permanently removes your profile, fan profile, answer and session history, marketing choices, friend graph, push token, and submissions
- **Export your data.** Email us and we will send you the data we hold for your account
- **Edit your fan profile.** Change your teams and age range, or change or clear your ZIP area, anytime in Settings → Your fan profile
- **Revoke permissions.** Notifications and Contacts permissions can be revoked at any time in iOS Settings → Roster Rivals
- **Ask a question.** Email us at the address below

---

## 7. Security

Passwords are hashed by our auth provider; we never see them. Data is transmitted to our backend over TLS. Account-level data is protected by row-level security policies in our database, meaning even our own backend code can only read data on behalf of an authenticated user.

No system is perfectly secure. If we discover a breach affecting your account, we will notify you by email.

---

## 8. Changes to this policy

If we change how we collect or use your data (for example, if a future version of Roster Rivals adds a new feature that collects new information), we will update this page and update the "Effective date" at the top. Material changes will also be communicated in-app or by email.

---

## 9. Contact us

For privacy questions, account deletion, or data export requests:

**rosterrivals@gmail.com**

We aim to respond within 7 days.

---

[← Back to main](index.html)
