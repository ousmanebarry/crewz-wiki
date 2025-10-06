# DB Schema

## Explanation

- **users** will be keeping track of user info and stats in general
- **friends** will be for creating a relationship between two users
- **convoys** will be for storing the fundamental info about a convoy
- **convoy_members** keeps track of all the people inside a convoy
- **convoy_stops** keeps track of potential stops added to a convoy
- **auth.users** is the default table created by supabase's authentication system

- **messages** is a supabase channel that will take care of broadcasting messages/alerts to other convoy members
- **locations** is a supabase channel that will take care of broadcasting locations to other users during a convoy

## Tables
  - users
  - friends
  - convoys
  - convoy_members
  - convoy_stops
  - auth.users (supabase auth table)
  
<img width="1390" height="737" alt="image" src="https://github.com/user-attachments/assets/6883c51e-347e-45c2-adaa-41a9801392d0" />

## Channels
  - messages
  - locations

<img width="546" height="504" alt="image" src="https://github.com/user-attachments/assets/86a69681-e0ec-471d-9083-e9e23e78e80c" />
