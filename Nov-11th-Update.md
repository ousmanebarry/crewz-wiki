# Added Profile Picture Upload/Management + working on location search & map setup using Google SDK

**Overview:**

Implements complete profile picture functionality allowing users to upload, view, and delete profile photos across web, iOS, and Android platforms (accepts only JPEG, JPG, and PNG images up to 5MB). Images are stored in Supabase Storage with automatic cleanup of old images. As for the location search, it will include a type of autocomplete when searching as well as input validation so users will not be able to put a random location that dosen't exist since we will be using google sdk to make sure it's an actual location we can set.

**Image Upload**

The image upload functionality takes care of uploading a new image when there is no current image as well as overwriting an image assuming there is one. It is a two to three step process:

- Firstly, we add the new image to the storage with a new path (userID+timestamp).
- Next, if there was already a profile pic for the current user in storage, we want to remove it using supabase's remove() storage function (if there's no profile pic then no need to complete this steps).
- Lastly, we have update the public.users supabase table by setting the current user's image_url value to the new image's path in storage so that it can be rendered in the UI. If user already had a profile pic before uploading a new pic we should find that image_url should be set to an existing URL in storage, if not, we should find a NULL value

**Image deletion**

The image deletion functionality takes care of deleting the current profile picture. It is a two step process:

- Firstly, we use supabase's remove() function to delete the image from storage (we obviously want to make sure we pass the image path in storage to the function).
- Next, we set the image_url in the public.users supabase table to NULL

**Expected Changes:**
- Ability to upload a new profile picture from scratch
- Ability to replace/overwrite current profile picture with a new one
- Ability to delete current profile picture
- Profile picture being rendered in multiple parts of the UI (user profile screen, convoy details screen, user's friends profile screen, etc.)
- Input validation for location
- Google SDK map integration