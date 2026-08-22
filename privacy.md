# Roadwave Privacy Policy

**Effective date:** 23 August 2026 (beta)
**Who is responsible:** Felix Tornberg, Sweden, the developer of Roadwave (the "data controller" under the GDPR)
**Contact:** roadwaveSupport@gmail.com

Roadwave is a voice chat app for people who are driving. It lets you talk to friends in a private channel (a Private Road) and to other drivers near you on an open channel (The Road). To do that it has to know where you are and stream your voice. This page explains exactly what the app collects, where it goes, how long it is kept, and what you can do about it. It is written to be read, not skimmed.

## The short version

- Roadwave has no accounts. You are identified by a random ID that the app makes up on your phone and a username you choose.
- While you are in a channel, your position is sent every 3 seconds to the Roadwave server and to the other drivers in that channel. When you leave, it stops.
- Your voice is streamed live to the other drivers in the channel. Roadwave does not record it.
- Nothing is sold, there are no ads, and there is no advertising or analytics tracking in the app.
- Write to roadwaveSupport@gmail.com to ask what we hold about you or to have it deleted.

## What the app collects and why

### Device ID
When you first open Roadwave, the app generates a random 32-byte identifier and stores it on your phone. It is not tied to your phone's hardware, your Apple or Google account, or anything else about you. The Roadwave server uses it to recognise the same install across requests, which is how it applies rate limits, checks that a position is plausible, and can suspend a device that has been reported. Reinstalling the app creates a new one.

### Username
The name you choose on first open (changeable in Settings). Other drivers see it next to your car and in their list. It is sent to the server with each channel you join, and it is the name a report about you would carry.

### Precise location
While you are in The Road or in a Private Road with location enabled, the app reads your GPS position about once a second and, every 3 seconds, sends your latitude, longitude, direction of travel and speed:

- **to the Roadwave server**, which uses it to place you in a road cell (an area roughly 4 km across) and to check that your movement is physically plausible. The server keeps only your most recent position, in memory, for up to 24 hours, and forgets it on every restart.
- **to the other drivers in your channel**, directly through the voice service, so their app can draw your car on their map and adjust your volume by distance. On The Road those drivers are strangers within a few kilometres of you. Blocked drivers do not receive your position.

Location sharing stops the moment you leave the channel. There is no background tracking when you are not in a call. The Road cannot be used without sharing your position: that is what the feature is.

### Voice
When your microphone is on, your voice is streamed live to the other drivers in your channel through LiveKit (see below). Roadwave does not record, store or transcribe voice, and has no access to it after it has been delivered. The microphone closes itself after 45 seconds of silence or 10 minutes of continuous use, and a bar across the screen shows whenever it is open.

### Vehicle choice
The car you pick in the Garage is sent to other drivers so they see the right car on the map. It is stored on your phone.

### Reports
If you report another driver, the app sends the Roadwave server their username, the channel you shared, the reason you chose, and your own device ID and username. The server emails that to roadwaveSupport@gmail.com, where a person reads it and decides what to do. Reports are the one thing that links a device ID to a human decision; they are kept in the support mailbox until they have been handled, then deleted.

### Blocked drivers and consent
The list of drivers you have blocked, and the fact that you have accepted The Road's disclosure, are stored on your phone only and never sent anywhere.

### Server logs
The Roadwave server writes a security log: one line per request type such as a session being issued, a channel being joined, a rate limit being hit, or a report being made. To keep this log from becoming a tracking database, it stores your IP address with the last part removed (for example 203.0.113.x) and any coordinates rounded to about 1 km. It is kept for up to 30 days on the hosting provider and then discarded.

## What the app does not collect

No contacts, no photos, no camera, no microphone use outside a channel, no background location, no advertising identifiers, no analytics or crash-reporting services, no payment details. The app does not read anything else on your phone.

## Who else handles your data

Roadwave runs on a small number of third-party services. Each sees only what it needs to do its job.

| Service | What it handles | Why |
|---|---|---|
| **LiveKit Cloud** (LiveKit, Inc., USA) | Your voice stream, your position messages, your username, your IP address | It is the voice service. Audio and position messages pass through its servers to the other drivers; it does not keep them. |
| **Railway** (Railway Corp., USA) | Everything the Roadwave server receives, including the security log | It hosts the Roadwave server. |
| **Google** (Gmail) | The contents of reports | Reports are delivered to the support inbox by email. |
| **OpenFreeMap** and **OpenStreetMap** | Requests for map tiles, which reveal roughly where your map is centred, and your IP address | They serve the map and the road data used to place cars on roads. Requests are only ever made around your own position, never around other drivers'. |
| **Apple** (TestFlight) and **Google** (Play, if used) | Your installation of the app | App distribution and crash reports under their own privacy policies. |

Some of these providers are in the United States. Where personal data leaves the EU/EEA it does so under the providers' standard contractual clauses.

Roadwave does not sell your data and does not share it with anyone else.

## How long things are kept

| Data | Where | For how long |
|---|---|---|
| Device ID, username, vehicle, blocked list, consent | Your phone | Until you uninstall the app |
| Session token | Your phone and the server | 30 days, then renewed |
| Your latest position | Server memory | Up to 24 hours, cleared on every restart |
| Voice and position messages | In transit only | Not stored |
| Security log | Hosting provider | Up to 30 days |
| Reports | Support mailbox | Until handled |

## Your rights

Under the GDPR you can ask to see the personal data held about you, to have it corrected or deleted, to restrict or object to its use, and to receive it in a portable form. Write to roadwaveSupport@gmail.com. Because Roadwave holds almost nothing about you that outlives a call, most requests come down to deleting the security log lines and any reports that name your device ID, and we will tell you what was found. You also have the right to complain to the Swedish Authority for Privacy Protection (Integritetsskyddsmyndigheten, IMY).

Deleting the app from your phone removes your device ID, username, blocked list and consent record. The server's copies expire on their own as described above.

## Children

Roadwave is made for people who drive and is not directed at children under 15. If you believe a person under the stated age is using it, write to the address above.

## Safety

Roadwave is meant to be used hands-free. The app is designed so that it never needs to be looked at while driving, but you are responsible for using it in a way that is legal and safe where you are.

## Changes

This policy will change as the app does, for example if reports move from email to a review tool. The effective date at the top moves when it does, and the app shows The Road's disclosure again whenever that text changes in substance.

## Legal basis (for the GDPR-minded)

Position and voice: performance of the service you asked for (Article 6(1)(b)). Device ID, rate limiting, plausibility checks, the security log and reports: our legitimate interest in keeping the service working and safe for other drivers (Article 6(1)(f)). Nothing here relies on consent that you could not withdraw simply by leaving a channel or deleting the app.
