# Added Profile Picture Upload/Management + working on location search & map setup using Google SDK

**Overview:**
Implements complete profile picture functionality allowing users to upload, view, and delete profile photos across web, iOS, and Android platforms (accepts only JPEG, JPG, and PNG images up to 5MB). Images are stored in Supabase Storage with automatic cleanup of old images. As for the location search, it will include a type of autocomplete when searching as well as input validation so users will not be able to put a random location that dosen't exist since we will be using google sdk to make sure it's an actual location we can set.

**Expected Changes:**
- Ability to upload a new profile picture from scratch
- Ability to replace/overwrite current profile picture with a new one
- Ability to delete current profile picture
- Profile picture being rendered in multiple parts of the UI (user profile screen, convoy details screen, user's friends profile screen, etc.)
- Input validation for location
- Google SDK map integration