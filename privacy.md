# Roadwave Privacy Policy

**Effective date:** 26 September 2026 (beta)
**Who is responsible:** Felix Tornberg, Sweden, the developer of Roadwave (the "data controller" under the GDPR)
**Contact:** roadwaveSupport@gmail.com

Roadwave is a voice chat app for people who are driving. It lets you talk to friends in a private channel (a Private Road) and to other drivers near you on an open channel (The Road). To do that it has to know where you are and stream your voice. This page explains exactly what the app collects, where it goes, how long it is kept, and what you can do about it. It is written to be read, not skimmed.

## The short version

- Roadwave has no accounts. You are identified by a random ID that the app makes up on your phone and a username you choose.
- While you are in a channel, your position is sent every 3 seconds to the Roadwave server and to the other drivers in that channel. When you leave, it stops.
- Navigation and the CarPlay map can also use your location without a voice channel. This does not share your position with other drivers.
- If you have accepted The Road's disclosure, connecting the app to CarPlay joins The Road for you, which starts sharing your position with nearby drivers as described below. Leaving the channel, from the car or the phone, stops it until the next time the car connects.
- Your voice is streamed live to the other drivers in the channel. Roadwave does not record it.
- If you navigate somewhere, the route is worked out on a Roadwave server and your destination is never written to any log. Searching for a place by name sends that text, via the Roadwave server, to Mapbox's place search, and nothing else about you.
- While the driving screen is open and you are moving, the app asks the Roadwave server for the speed limit of the road you are on, sending the last few seconds of your position. Nothing about that lookup is stored or logged. Fixed speed camera positions come from Trafikverket's open data; nothing about you goes to Trafikverket.
- The map, on the phone and on the CarPlay screen, is drawn by Mapbox, which also collects anonymised usage statistics unless you switch that off in the ⓘ menu on the map.
- Nothing is sold, there are no ads, and there is no advertising tracking in the app.
- Write to roadwaveSupport@gmail.com to ask what we hold about you or to have it deleted.

## What the app collects and why

### Device ID
When you first open Roadwave, the app generates a random 32-byte identifier and stores it on your phone. It is not tied to your phone's hardware, your Apple or Google account, or anything else about you. The Roadwave server uses it to recognise the same install across requests, which is how it applies rate limits, checks that a position is plausible, and can suspend a device that has been reported. Reinstalling the app creates a new one.

### Username
The name you choose on first open (changeable in Settings). Other drivers see it next to your car and in their list. It is sent to the server with each channel you join, and it is the name a report about you would carry.

### Precise location
While you are in The Road or in a Private Road with location enabled, the app reads your GPS position about once a second and, every 3 seconds, sends your latitude, longitude, direction of travel and speed:

- **to the Roadwave server**, which uses it to place you in a road cell (an area roughly 4 km across) and to check that your movement is physically plausible. The server keeps only your most recent position, in memory, for up to 24 hours, and forgets it on every restart. It also remembers which road cell you are in, and which Private Road you have open, for about 90 seconds, so that it can tell another driver's phone whether anybody is there before that phone connects to the voice service. That answer is only yes or no; it never says who, or where. Leaving The Road clears it at once.
- **to the other drivers in your channel**, directly through the voice service, so their app can draw your car on their map and adjust your volume by distance. On The Road those drivers are strangers within a few kilometres of you. Blocked drivers do not receive your position. When voice is paused, or in the moment before your phone connects to them, your position reaches the same drivers through the Roadwave server instead: it passes the position on, keeps only the latest one in memory for about 15 seconds, and sends it to nobody who has blocked you or whom you have blocked.

Location sharing with other drivers stops when you leave the channel. Navigation and the connected CarPlay map can continue using location, including while the phone is locked or another app is open. To stop that use outside a channel, end navigation and disconnect CarPlay. The Road cannot be used without sharing your position: that is what the feature is.

When the app is connected to CarPlay it joins The Road automatically, so that a drive can start hands-free. This only happens if you have already read and accepted The Road's disclosure on the phone, and it starts the same position sharing described above. You can leave The Road from the car screen or the phone at any time; the app will not rejoin on its own until the next time the car connects.

### Where you are going (navigation)
If you use navigation, the app sends the Roadwave server your current position and the destination you chose, and gets back a route. The route is calculated on a Roadwave-operated server; it is not sent to any mapping company.

The phone and CarPlay share the same navigation session. Leaving a voice channel while CarPlay is connected does not end navigation. Route requests, including rerouting requests, send the position and destination needed to calculate the route. GPS updates used to advance navigation are not shared with other drivers unless you are also in a voice channel.

Your destination is **never written to the server's log**, at any precision. This is stricter than the rule for ordinary positions above, because a destination says where you will be later rather than where you are now. The log records only the length of the route in whole kilometres and how many turns it has.

When you search for a place by name, the text you type is sent to the Roadwave server and forwarded to **Mapbox's search service**, together with a position the server first rounds to about a kilometre so that results near you come first. Mapbox receives nothing else from that request: no device ID, no username, no route, and never the destination you go on to pick. The search text is not logged by the Roadwave server.

The last few places you navigated to are stored **on your phone only** and are never sent anywhere. Deleting the app deletes them.

You can send your route to another driver in your channel. What is sent is the destination and any stops, by name and position, directly to that one driver through the voice service — not through the Roadwave server, and never your current position beyond what the channel already shares. They see who it is from and choose whether to follow it. If you change the route afterwards, the update goes to the same drivers. Nothing is sent to anyone you have blocked, or who has blocked you.

### Voice
When your microphone is on, your voice is streamed live to the other drivers in your channel through LiveKit (see below). Roadwave does not record, store or transcribe voice, and has no access to it after it has been delivered. The microphone stays off until you turn it on, stays on until you turn it off, and a bar across the screen shows whenever it is open.

### Vehicle choice
The car you pick in the Garage is sent to other drivers so they see the right car on the map. It is stored on your phone.

### Reports
If you report another driver, the app sends the Roadwave server their username, the channel you shared, the reason you chose, and your own device ID and username. The server emails that to roadwaveSupport@gmail.com, where a person reads it and decides what to do. Reports are the one thing that links a device ID to a human decision; they are kept in the support mailbox until they have been handled, then deleted.

### Blocked drivers and consent
The list of drivers you have blocked, and the fact that you have accepted The Road's disclosure, are stored on your phone only and never sent anywhere.

### Server logs
The Roadwave server writes a security log: one line per request type such as a session being issued, a channel being joined, a rate limit being hit, or a report being made. To keep this log from becoming a tracking database, it stores your IP address with the last part removed (for example 203.0.113.x) and any coordinates rounded to about 1 km. It is kept for up to 30 days on the hosting provider and then discarded.

## What the app does not collect

No contacts, no photos, no camera, no microphone use outside a channel, no advertising identifiers, no crash-reporting services, no payment details. Location may continue for an active channel, navigation or connected CarPlay as described above. Mapbox's map telemetry is described below and can be turned off.

## Who else handles your data

Roadwave runs on a small number of third-party services. Each sees only what it needs to do its job.

| Service | What it handles | Why |
|---|---|---|
| **LiveKit Cloud** (LiveKit, Inc., USA) | Your voice stream, your position messages, your username, your IP address | It is the voice service. Audio and position messages pass through its servers to the other drivers; it does not keep them. |
| **Railway** (Railway Corp., USA) | Everything the Roadwave server receives, including the security log | It hosts the Roadwave server. |
| **Google** (Gmail) | The contents of reports | Reports are delivered to the support inbox by email. |
| **Mapbox** (Mapbox, Inc., USA) | Requests for map tiles and 3D buildings, which reveal roughly where your map is centred, and your IP address. Also, unless you turn it off, anonymised map-usage telemetry that can include your location while the map is open. | It draws the map on the phone, on the CarPlay screen and in the CarPlay Dashboard. Mapbox's software collects telemetry by default to improve its maps; the ⓘ button on the map opens Mapbox's own menu where you can switch this off, and that choice is kept on your phone. Roadwave itself never receives that telemetry. |
| **Mapbox** search (same company) | The text you type when searching for a place, and a position rounded to about 1 km by the Roadwave server | It turns a place name into coordinates. It never receives your device ID, your username, your route, or the destination you choose. |
| **Apple** (CarPlay) | The turn instructions, distances, search text and channel names shown on the car screen pass through Apple's CarPlay framework on your phone. Roadwave sends nothing to Apple's servers for this. Only if the Mapbox map cannot be loaded does the car screen fall back to Apple's MapKit map, which then requests map tiles from Apple under Apple's Maps privacy terms. | It is how any app appears on a car's screen. |
| **OpenFreeMap** and **OpenStreetMap** | Requests for road-data tiles, which reveal roughly where you are, and your IP address | They provide the road centrelines used to place cars on roads. Requests are only ever made around your own position, never around other drivers'. |
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
| Your last few seconds of position, for the speed limit | In transit only | Not stored, not logged |
| Private Roads you are in | Server database | Until you leave the road, or nobody uses it for 90 days |
| Hazards you report | Server database | Between 20 minutes and 24 hours depending on the kind, then swept |
| Security log | Hosting provider | Up to 30 days |
| Reports | Support mailbox | Until handled |

Two of those outlive a call, and both are new since this policy was first
written.

**Private Roads.** A road is saved so you can get back on it, which means the
server keeps a row per road (its name, its code and its settings) and a row per
member (a device ID, the username that device was using, and when it last
joined). Other drivers in a road see your username and a short scrambled tag,
never your device ID. Leaving a road deletes your membership. If you made the
road, leaving deletes the road itself.

**Hazards.** A hazard is stored with its position and the device that reported
it. **The reporting device is never sent to any other driver** — it is there so
the same phone cannot report the same thing repeatedly or vote on it twice, and
it goes when the hazard is swept.

**Speed limit.** While the driving screen or CarPlay is open and the car is
moving, the app sends the Roadwave server the last few seconds of your position
(two to eight points), roughly every five seconds, to look up the speed limit of
the road you are on. The server passes them to its own routing service, which
is operated by Roadwave, answers with the limit, and keeps nothing: the lookup
is not stored and not written to the security log.

**Fixed speed cameras.** The positions of Sweden's fixed speed cameras come from
Trafikverket's open data, which the server fetches once a day. Nothing about you
is sent to Trafikverket.

## Your rights

Under the GDPR you can ask to see the personal data held about you, to have it corrected or deleted, to restrict or object to its use, and to receive it in a portable form. Write to roadwaveSupport@gmail.com. Roadwave holds very little about you that outlives a call: your memberships of the Private Roads you are in, any hazards you have reported that have not yet expired, the security log lines, and any reports that name your device ID. A deletion request comes down to those, and we will tell you what was found. You also have the right to complain to the Swedish Authority for Privacy Protection (Integritetsskyddsmyndigheten, IMY).

Deleting the app from your phone removes your device ID, username, blocked list and consent record. Because there are no accounts, a fresh install is a new device that cannot get back into the roads the old one was in. The server's copies expire on their own as described above.

## Children

Roadwave is made for people who drive and is not directed at children under 15. If you believe a person under the stated age is using it, write to the address above.

## Safety

Roadwave is meant to be used hands-free. The app is designed so that it never needs to be looked at while driving, but you are responsible for using it in a way that is legal and safe where you are.

## Changes

This policy will change as the app does, for example if reports move from email to a review tool. The effective date at the top moves when it does, and the app shows The Road's disclosure again whenever that text changes in substance.

## Legal basis (for the GDPR-minded)

Position and voice: performance of the service you asked for (Article 6(1)(b)). Device ID, rate limiting, plausibility checks, the security log and reports: our legitimate interest in keeping the service working and safe for other drivers (Article 6(1)(f)). Nothing here relies on consent that you could not withdraw simply by leaving a channel or deleting the app.
