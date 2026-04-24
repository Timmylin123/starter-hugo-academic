---
title: Timmy in Crerar
date: 2026-04-23T19:10:00.000Z
draft: false
featured: false
links:
 - name: Open Dashboard
   url: uploads/timmy_in_crerar.html
---
Timmy in Crerar is a lightweight location-intelligence project: a mobile app collects validated presence signals at John Crerar Library, a backend stores clean session data, and this website publishes a read-only public dashboard.

Architecture highlights:
- Phone app (React Native + Expo) is the data collector.
- GPS and geofence logic run on-device to detect when Timmy enters/leaves Crerar.
- The app is designed to ship as a real standalone build (not only Expo Go) so tracking can continue without a laptop or local dev server.

- Small backend (Supabase style) is the source of truth.
- Sessions are stored as structured records: `start`, `end`, `duration`, and status transitions.
- Day/week/month totals are derived from the session table for consistency across all clients.
- Access uses a single private user identity/token (personal-use workflow).

- Website is a read-only display layer.
- The site fetches aggregate stats and weekly chart data from backend views/RPC endpoints.
- No browser location permissions are required, because the web page never collects GPS.
- Result: fast public visibility of live work stats while keeping collection logic in the phone app.
