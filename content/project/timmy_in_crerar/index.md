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

A React Native app (via Expo Go / standalone build) runs on the phone to track geolocation and detect entry/exit using on-device geofencing, then sends structured session data (start, end, duration, status) to a Supabase backend that serves as the single source of truth. The website fetches aggregated stats from the backend and displays them as a live dashboard without needing any location permissions.

Current limitation: during development the app depends on npm start (Expo dev server), and background tracking may stop unless the app is built and configured as a standalone app.
