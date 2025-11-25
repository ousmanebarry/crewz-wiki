# Working on Convoy Implementation Functionality + Enhancing user profile search (None of them complete yet)

## The goal is to have the entire convoy feature working end-to-end in the next couple of weeks. This includes:

**Convoy Creation & Scheduling**
- Users can create a convoy with a destination, optional stops, and a scheduled start time.

**Friend Invitations & Responses**
- Users can invite friends to join their convoy, and friends can accept or decline invitations.

**Real-Time Convoy Tracking**
- Every participant’s location is updated live on a shared map using Google Maps SDK.
- Users can see who has joined, who hasn’t, and who leaves during the convoy.

**Starting & Ending Convoys**
- Convoys can be started by the creator.
- Real-time data continues to track users throughout the journey.
- Convoys can be ended, finalizing status and optionally updating convoy statistics.

**Enhancing User Profile Search**
The goal is to create a more fluid/intuitive search experience, inspired by modern social media applications (like instagram or snapchat). Improvements include:

- Searching users by username (possibly include email option)
- Displaying relevant results with profile pictures and basic info (we query the db as the user searches instead of requiring the exact username match).
