Product Requirements Document (PRD) — catchGPT MVP (Phase 1)

1. Product Vision

To make Ganpati Darshan discovery simple, quick, and shareable for users by providing a map-based interface with nearby listings of Ganpati mandaps/pandals, accessible via a mobile-friendly web app.

2. Goals

Help users find the nearest Ganpati pandals with directions.

Provide shareable links so users can coordinate with friends/family.

Lay the groundwork for crowdsourced and committee-submitted listings in later phases.

3. Target Users

Festival visitors: looking for nearby pandals.

Families/groups: want to plan routes together.

Organizers (in future): want visibility for their pandal.

4. Core User Features (Must-Have)

✅ Location Detection & Nearby Map Pins

Auto-detect user location.

Show pins for nearby Ganpati pandals on a map.

✅ Pandal Listing (Basic Info)

Each pin shows:

Pandal name

Location/address

Category tag (e.g., “Famous”, “Eco-Friendly”)

Photo (optional for Phase 1, but great if possible)

✅ Search & Filter

Search by area/locality.

Filters: Famous Pandals, Community Pandals, Eco-friendly.

✅ Directions

One-tap "Get Directions" → Opens in Google Maps app.

✅ Shareability

Each pandal/location has a unique URL (deep link).

"Share this Pandal" button → WhatsApp, SMS, social.

5. Future (Phase 2+) Nice-to-Have (Not in MVP)

Queue wait time status.

Live photos or theme updates.

User ratings & reviews.

Gamification (check-ins, darshan badges).

6. Tech Stack (Lean & Fast)

Frontend (Web-App):

React (Next.js for SSR & SEO) with Typescript

TailwindCSS (fast styling)

Mobile-first PWA (works like app, installable on phones)

Maps Integration:

Google Maps JavaScript API (for embedding + pins)

Google Places API (for base map/location services)

Backend (for listings DB):

Firebase (Firestore for fast cloud DB + Auth if needed later)

Firebase Hosting (cheap, scalable hosting)

Cloud Functions (if needed for API layer)

Data Source (MVP):

Seed with curated dataset of popular pandals (scraped/partner with local committees).

Manual CSV upload → populate DB.

A quick Google integration to upload individual entries

7. User Experience Flow
   Entry

User clicks shared link / opens web app.

Homepage → “Find Ganpati Near Me” (location permission).

Discovery

Map view opens → auto-pins nearby pandals.

Sidebar/list view (optional toggle): thumbnails of pandals.

Tap on a pin → bottom sheet opens with:

Name

Address

“View More” → detailed page (optional in MVP)

Action

CTA Buttons on Pandal detail:

“Get Directions” → Google Maps

“Share” → system share menu (WhatsApp, etc.)
