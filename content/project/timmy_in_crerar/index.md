---
title: Timmy in Crerar
date: 2026-04-23T19:10:00.000Z
draft: false
featured: false
links:
 - name: Open Dashboard
   url: uploads/timmy_in_crerar.html
---
Timmy in Crerar is a lightweight location-intelligence project: a Chrome extension collects Crerar presence signals from Timmy's laptop, a backend stores clean session data, and this website publishes a read-only public dashboard. 

A Chrome extension checks whether the laptop's public IP matches known Crerar/UChicago network rules, then sends structured session data and heartbeat presence updates to a Supabase backend that serves as the single source of truth. The website fetches aggregated stats from the backend and displays them as a live dashboard without needing any location permissions.

Current limitation: Chrome does not guarantee a final network request when the browser or laptop closes, so the dashboard treats stale heartbeats as offline.
