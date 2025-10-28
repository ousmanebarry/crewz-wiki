# User Sign up, Login, Account Confirmation, Friend connection, and convoy creation Complete


**User Authentication Flow**

1. Sign Up
- New users can create an account by signing up on the signup screen using their email, username, and password.

- Upon successful registration, a confirmation email is automatically sent to the user’s email address.

- Users are redirected to an Email Confirmation screen where they’re guided to verify their account (this includes steps like where to go and what to do).

2. Email Confirmation

- Supabase automatically sends a confirmation link to the email account the user registered with.

- Users cannot log in until their email is verified (if they try, they will receive a pop letting them know their account isn't confirmed yet and giving them the option to either close the Alert or click the resend email button which once again redirects them to email confirmation screen).

- The Resend Confirmation Email” button allows users to resend the confirmation email if the first one failed or expired.

- They can access it both from the confirmation screen and the login alert when trying to log in without a verified account.

3. Login

- Registered AND confirmed users can log in using their registered email/username and password.

- Login errors are displayed clearly to guide the user (e.g., invalid credentials, unconfirmed account).

- Implemented redirect to main dashboard upon successful authentication.


**Friend Connection System**

- Users can now send and accept friend requests.


**Convoy Creation**

- Users can create a convoy (group ride) with selected friends.

- Convoy creator becomes the host and can manage participants (can start or end or cancel convoy).

- Basic convoy metadata (title, participants, status) is stored and retrievable (implemented dashboard showing upcoming/completed convoys).


**Next Steps**

- Add user profile customization (avatars, bios, etc.).

- Introduce notifications for friend requests and convoy invites.

- Implement convoy chat feature.

- Implement convoy map using Google maps sdk