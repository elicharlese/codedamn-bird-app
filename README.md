# codedamn-bird-app

Hello there, welcome to the first step of the making bird app social media project. The aim for this project is to build a simple CRUD app for manipulating social media posts but only with localStorage knowledge.

## Build a landing page for the social media

This step involves you building a landing page for the social media website. Take a look inside the task checklist on the left to see all the steps you have to complete to pass this step.

In this step, we will aim to build a register page on /register path. You will have to work with `localStorage` API to add the registered user to `localStorage` once they register successfully.

## Pointers to note

-   This is how the schema for localStorage could look like:

```json
[
	{
		"username": "admin",
		"password": "123"
	},
	{
		"username": "john",
		"password": "456"
	}
]
```

-   Add basic validation to the registration: Usernames should be unique, alphanumeric only. Passwords should be strong.

In this step, the main goal is to build the /login page to extend functionality of the /register page. Your users should be able to login with the same credentials.

Check the challenges tabs to know what all you should be implementing. All the best!

The dashboard should load feed from all the users. This feed should be also stored in localStorage as feed as the localStorage key, and the following structure as the value (feel free to change it to add more features):

```json
[
	{
		"postID": "", // a unique post ID
		"contents": "", // contents of the post
		"postAuthor": "", // username of the author of the post
		"createdOn": 0, // a unix timestamp (stored in seconds) of the time it was created
		"updatedOn": 0 // a unix timestamp (stored in seconds) of time it was updated
	}
]
```

-   Whenever a user creates a new post, it is added into the `localStorage` key feed as an individual post.
-   All posts inside feed `localStorage` should be visible to everyone in random order who create an account and visits `/dashboard`
-   Only the post author should see the option to edit or delete the post.
-   Only the post author can edit and delete the post. Put proper checks in place.
-   Take design inspiration from assets folder, but you have to build the design + logic on your own.
