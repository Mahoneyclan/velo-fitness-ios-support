# Velo Fitness privacy policy

Effective date: November 2026

**The short version:** Velo Fitness stores all your data locally on your device. The developer runs no server and collects nothing. The app talks only to Strava and Garmin, plus one public file server needed for Garmin sign-in (described below), and only when you sign in or sync.

## What data the app accesses

Velo Fitness connects to the following external services only when you start a sync:

- **Strava:** cycling activity metadata (name, date, distance, time, elevation, heart rate, power, cadence, speed), fetched through the official Strava API using OAuth 2.0.
- **Garmin Connect (beta):** the same cycling activity fields, plus, for boxing workouts, the original activity file (FIT file) your watch uploaded. The app reads heart rate, calories, duration and the punch metrics recorded by the f3b Boxing app from it. Fetched with your Garmin email and password through Garmin's mobile sign-in. This integration is unofficial and not affiliated with Garmin Ltd.

No other data sources are accessed. The app does not access your location, camera, contacts, photos, microphone or any other device capability.

## How data is stored

- All ride data is stored locally on your device in the app's private Documents folder as `rides.json`. Boxing sessions are stored the same way in `boxing_sessions.json`. Downloaded FIT files are read in memory and not kept.
- Strava sign-in tokens (access token, refresh token, expiry) are stored encrypted in the iOS Keychain, on this device only. They are not included in backups.
- Garmin sign-in tokens and the email address you signed in with are stored encrypted in the iOS Keychain, on this device only. Garmin's sign-in cookies are kept in the app's private cookie store. Your Garmin password is used only during sign-in and is never stored by this app.
- Your activity files in the Documents folder are included in your device backups (iCloud or computer) like other app data. Sign-in tokens are not, so after restoring onto a new device you sign in again.
- No data is stored in iCloud, on any external server, or in any database operated by this app's developer.

## Data sharing and third parties

Velo Fitness does not:

- sell, share or transmit your data to any third party
- use analytics or crash-reporting services
- display advertising
- track you across apps or websites

The app only makes network requests when you sign in or sync, and only to:

- **www.strava.com** (Strava, Inc., USA): Strava sign-in and activities.
- **sso.garmin.com** and **connectapi.garmin.com** (Garmin Ltd.): Garmin sign-in, activities and FIT file downloads.
- **thegarth.s3.amazonaws.com:** a public file hosted on Amazon Web Services (USA) by the open-source garth project. On your first Garmin sign-in the app downloads Garmin's app sign-in keys from it. No personal data is sent, but like any web server it can see your device's IP address.

## Strava data

By connecting your Strava account you agree to Strava's Terms of Service and Privacy Policy. You can revoke Velo Fitness's access to your Strava account at any time at strava.com/settings/apps.

## Garmin data (beta)

The Garmin integration uses an unofficial API and is provided as a beta feature. It is not endorsed by or affiliated with Garmin Ltd. By using this feature you accept that it may stop working at any time and that your use is subject to Garmin's Terms of Service.

## Data deletion

To delete all data collected by this app:

- In the app, tap the gear on either tab, then **Delete All My Data**. This removes every ride and boxing session from your device, deletes your sign-in tokens, email and cookies, and asks Strava to remove the app's access. Your activities on Strava and Garmin aren't affected.
- Or delete the app from your device. This removes `rides.json` and `boxing_sessions.json`. iOS may keep the encrypted sign-in tokens in the Keychain, but the app deletes them the next time it is installed, before anything can use them.
- Signing out of Strava inside the app also asks Strava to remove the app's access. Signing out of Garmin removes its tokens, email and sign-in cookies. Both keep your synced activities.
- To check or revoke Strava access yourself, visit strava.com/settings/apps.

## Children's privacy

Velo Fitness is not directed at children under 13. We do not knowingly collect any information from children.

## Changes to this policy

If this policy changes materially, the effective date above will be updated. Continued use of the app after a policy update constitutes acceptance of the revised terms.

## Contact

Questions about this privacy policy? Email [mahoneyclanapps+velofitness@gmail.com](mailto:mahoneyclanapps+velofitness@gmail.com).

Not affiliated with Strava, Inc. or Garmin Ltd.
