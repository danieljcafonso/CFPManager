# CFPManager :desktop_computer:
Do you find yourself often having all your CFP spread around various places? Would you like to have a dedicated space where you can create and manage all your CFP? I sure do!

CFPManager is a project that will allow you to list, create, and edit all your CFP while also keeping track all of the conferences you applied to with that CFP. You will also be able to see your friends CFPs if they choose to share them.

## Users of the app :technologist:

There are two users of the app: the authenticated user and the non authenticated user.
### Non Authenticated User
This user should be able to see a list of users of the app that have public CFP
### Authenticated User
This user should be able to do everything a non-authenticated user does. 
This user should be able to create, edit, view and delete CFP.

## Features :thinking:
### Access to Notion account or Login
To use the app you need to give it access to your Notion page.
If Notion API doesn't support all the use cases I have then instead I'll use Auth0 React SDK for managing login

### Dashboard
If logged in you should be able to:
- See all your CFP.
- Add a new CFP or edit previous ones. 
- Delete your CFP.
- You can also add new conferences and link CFP to them as submitted or approved.
- See random users with public CFP
If not logged you should be able to:
- See random users with public CFP

### Creating a new CFP
In this feature you will have access to a form with all the common questions asked in a CFP about your talk. This form will also include required fields and validations on the fields.

### Managing a new CFP
Here you will have access to the same form above but with all the data previously submitted pre filled in. Now you can edit your CFP. (Ideally in the future we have an history of changes on the same CFP).

### Viewing a CFP
In this feature you should be able to see your CFP and copy each individual field to the clipboard.

### Profile
In the profile you can see all the user public CFP

### Export to Notion (Optional)
If Notion API doesn't fit the initial use case I'd like it at least to be able to export my CFP to Notion as a backup

## Expected Tech Stack :grey_question:
- Notion API for managing authorization and hosting CFP or Database in Supabase and Auth0 React SDK
- TypeScript because reasons
- React Hook Form for managing forms
- React Query for managing server state
- XState for managing application state
- Yup for validations
- Netlify for hosting
- RTL/Cypress for testing (optional)

## Other notes

Will work with a Kanban methodology to be able to prioritize my features backlog and limit the work in progress.
