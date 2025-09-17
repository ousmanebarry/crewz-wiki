## What is Crewz

Crewz is a mobile app that helps drivers create, join, and coordinate real life convoys.
The goal is to make group drives safer, more organized, and more fun by offering:

- Live location sharing (only while the convoy is active)

- A shared map that shows all drivers in the group

- Simple communication tools like chat and alerts

## Tech Stack

- Frontend: React Native

- Backend / Database: Supabase + TypeScript (Express.js for APIs)

- Maps & Live Location: Google Maps SDK + Supabase Channels

- Authentication: Supabase (email or phone login)

## Features (Main features + extra possible features if time allows)

- Convoy Creation & Joining
    - Create a convoy with a set destination (and optional stops).
    -Invite others as friends (will either use shared link or will give users ability to befriend other users like on instagram and other social media apps).
    -Live locations are shared only once the convoy starts.

- Real-Time Convoy Tracking (Map)
     - Show all joined drivers on a shared map like a video game (Forza, F1, Mario kart).
     - Indicate if a driver hasn’t joined yet or has left.
     - Reroute user who’s not within convoy circle to intersect at a certain point and rejoin the convoy (either that or reroute to convoy destination).
 
- Convoy Communication
     - Group chat for convoy members.
     - Basic alerts (e.g., “Route change”, “Stopping soon”).

- Convoy Dashboard
     - List active and upcoming convoys.
     - Show who’s in and convoy status.




