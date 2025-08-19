# catchGPT MVP - Project Plan & Todo List

## Project Plan

Based on the `prd.md` and `schema.md`, this plan outlines the steps to build and deploy the MVP for catchGPT. The goal is to create a mobile-friendly web app for discovering Ganpati pandals.

### Key Assumptions & Decisions

1.  **Initial Data Seeding**: The MVP will use a CSV file to seed the initial pandal data into Firestore. A script will be created for this purpose.
2.  **API Keys**: The project will require API keys for Google Maps (Maps JavaScript API, Places API) and a Firebase project configuration. These will need to be set up by the project owner.
3.  **Search Implementation**: Search by area/locality will use the Google Places API for autocomplete functionality.

## Todo List

### Phase 1: Project Setup

- [ ] Initialize Next.js project with TypeScript and Tailwind CSS
- [ ] Set up Firebase project (Firestore, Hosting) and configure in the app
- [ ] Set up Google Maps API and integrate it into the app

### Phase 2: Backend & Data

- [ ] Create a script to seed Firestore with pandal data from a CSV file

### Phase 3: Core Features

- [ ] Implement map view to display pandal markers from Firestore
- [ ] Implement user location detection to center the map
- [ ] Implement a detail view (bottom sheet/modal) for a selected pandal
- [ ] Implement search by area/locality
- [ ] Implement filtering by tags
- [ ] Implement "Get Directions" and "Share" functionality
- [ ] Create unique, shareable URLs for each pandal

### Phase 4: PWA & UI/UX

- [ ] Configure the app as a Progressive Web App (PWA)
- [ ] Ensure the UI is mobile-first and responsive

### Phase 5: Deployment & Testing

- [ ] Deploy the application to Firebase Hosting
- [ ] Conduct end-to-end testing of the MVP
