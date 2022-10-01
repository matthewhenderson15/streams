Streams

This application is a clone of Twitch. The application features the following architecture:
- React application which will allow users to add, edit, delete, and view channels
- A web server which knows which streams are currently broadcasting
- A Real Time Messaging Protocol server (RTMP)

User Experience
- User can see a list of available streams whether logged in to the application or not
- The user then selects a stream to view 
- This action then sends off a request to the RTMP server to render the video that was selected

Notable features
- Navigation is handled using React Router to control what content is rendered based on specific route
- Authentication is handled using Google oAuth
- State is managed using Redux and Redux Forms to make the process of dispatching actions and updating state of components simpler

Main Routes
1) Main landing page - displays initial content when user is not logged in
2) Page to render video content to user
3) Landing page which displays different content if the user is logged in
4) Form to create, edit, or delete a stream

Google Authentication
- Component stores the sign-in status of the user as state
- Helper methods defined to sign user in, sign user out, modify state, and render correct auth button (sign-in or sign-out)
