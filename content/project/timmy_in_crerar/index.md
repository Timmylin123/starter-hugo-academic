---
title: Timmy in Crerar
date: 2026-04-23T19:10:00.000Z
draft: false
featured: false
links:
 - name: Open Dashboard
   url: uploads/timmy_in_crerar.html
---
Timmy in Crerar is a lightweight presence-tracking project: a Chrome extension running in Timmy’s school Chrome profile checks whether his laptop is active on eduroam / UChicago network conditions associated with Crerar, a Supabase backend stores clean heartbeat and session data, and this website publishes a read-only public dashboard. The purpose of this mini-project is to encourage everyone to come in person to Crerar and build a steady work routine.

Current limitation: I first attempted to use phone-based geolocation through an Expo app, but Expo Go was not reliable for this use case because the app could stop tracking after refreshes, background execution was uncertain, and relaunching the tracker often depended on running the Expo dev server from a laptop. The current Chrome-based version avoids that workflow, but it still identifies Crerar presence through Chrome activity and network/IP matching rather than GPS or building-level Wi-Fi detection.
