# Facebook Clone — Practice Project

## Project Overview

This project is a practice implementation of a social networking website inspired by Facebook. The goal is to learn how a modern social media application is structured and how its front end, back end, database, and authentication work together.

This is an independent educational project. It is not affiliated with, endorsed by, or an official product of Meta or Facebook. Use your own name, branding, graphics, and sample data when extending it.

## Main Learning Goals

- Practice Git and GitHub workflows by cloning a repository, creating branches, committing changes, and pushing updates.
- Understand how a social media interface is organized into reusable components.
- Build responsive layouts for desktop, tablet, and mobile screens.
- Learn how users, posts, comments, reactions, and friendships or follows can be represented in a database.
- Practice authentication, authorization, form validation, and error handling.
- Learn to connect a front end to APIs and manage loading, success, and failure states.
- Improve code readability, debugging, and project documentation.

## Possible Features to Practice

The features below are ideas for learning and may not all exist in the current repository. Check the source code before assuming a feature has already been implemented.

### 1. User Interface

- Navigation bar with a search field and account controls.
- Sidebar with profile information and navigation links.
- Feed area displaying posts.
- Right-side panel for suggested contacts or other useful information.
- Responsive layout that adapts to smaller screens.
- Reusable components for buttons, cards, menus, and dialogs.

### 2. User Profiles

- Display name, profile image, cover image, and short biography.
- Profile page showing a user's posts.
- Edit-profile form with input validation.
- Optional privacy settings for profile information.

### 3. Posts and Feed

- Create a text post.
- Display posts with author details and timestamps.
- Edit or delete your own posts.
- Add image uploads after validating file type and size.
- Sort feed items by creation time.
- Show an empty state when there are no posts.

### 4. Reactions and Comments

- React to a post and remove or change a reaction.
- Display a reaction count.
- Add comments to a post.
- Edit or delete your own comments.
- Validate comment text and handle failed API requests.
- Prevent duplicate reactions from the same user if the data model supports that rule.

### 5. Connections

- Send, accept, or decline connection requests.
- Remove an existing connection.
- Show a list of friends or followed users.
- Add search and suggestions as a later exercise.

### 6. Authentication and Security

- Register and log in using a secure authentication flow.
- Log out and handle expired sessions.
- Protect pages or API endpoints that require authentication.
- Validate user input on both the client and server.
- Store passwords using a suitable password-hashing algorithm if implementing your own backend.
- Never put private keys, passwords, API secrets, or production credentials in the repository.
- Use environment variables for secrets and keep local `.env` files out of Git.

### 7. Notifications and Messaging

These are optional, more advanced extensions:

- Notify a user when someone reacts to or comments on their post.
- Show pending connection requests.
- Build a basic one-to-one messaging interface.
- Add unread-message counts.
- Explore real-time updates only after the basic API and data model work reliably.

## Suggested Development Roadmap

### Stage 1 — Explore the Existing Repository

1. Open the project folder in your editor.
2. Read `README.md`, `package.json`, and the folder structure.
3. Identify the framework, entry point, routes, components, and styling approach.
4. Install dependencies using the package manager and lockfile already used by the project.
5. Run the project and record which features currently work.
6. Check the browser console and terminal for errors.

### Stage 2 — Understand the UI

1. Identify the main layout components.
2. Trace how data reaches each component.
3. Find repeated UI and consider extracting reusable components.
4. Test the layout at different screen widths.
5. Improve accessibility with labels, semantic elements, and keyboard-friendly controls.

### Stage 3 — Add CRUD Practice

CRUD means Create, Read, Update, and Delete.

- Create: add a post or comment.
- Read: display posts and profile data.
- Update: edit a post or profile.
- Delete: remove a post or comment that belongs to the current user.

Start with one feature and test all four operations before moving on.

### Stage 4 — Connect an API and Database

If the project has a backend, inspect its routes, controllers, models, and middleware. If it is currently front-end only, you can first use mock data, then build a small API as a separate learning step.

For each API operation, document:

- HTTP method and endpoint.
- Required authentication.
- Request body or URL parameters.
- Successful response.
- Possible error responses.
- Authorization rules.

### Stage 5 — Test and Refine

- Test valid and invalid form submissions.
- Test loading, empty, success, and error states.
- Test what happens when a request fails.
- Confirm that one user cannot edit or delete another user's content.
- Check responsive behavior and accessibility.
- Remove unused code and document setup instructions.

## Example Git Workflow

Check your current branch and working tree:

```bash
git status
git branch
```

Create a feature branch before making a change:

```bash
git switch -c feature/post-comments
```

After implementing and testing the feature:

```bash
git add .
git commit -m "Add post comments"
git push -u origin feature/post-comments
```

Use meaningful commit messages that describe the change. Review `git status` before committing so you do not accidentally include unrelated files or secrets.

If you are practicing on a repository you do not own, you may not have permission to push to its original remote. In that case, fork it to your own GitHub account and push to your fork.

## Suggested Practice Tasks

Try these tasks in order:

1. Change the page title and document the change.
2. Improve one responsive layout issue.
3. Add a clear empty-feed message.
4. Add client-side validation to the post form.
5. Add a character counter for post text.
6. Implement comments with mock data or an API.
7. Add edit and delete controls with ownership checks.
8. Add loading indicators and error messages.
9. Write tests for a small component or API route.
10. Update this document with the features you actually implemented.

## Definition of Done

A practice task is complete when:

- The feature works in the normal case.
- Invalid input is handled gracefully.
- Loading and error states are understandable.
- The layout works at common screen sizes.
- Existing features still work.
- Changes are committed with a clear message.
- The documentation reflects the current behavior.

## Important Note

This document is a learning plan and project description, not a claim that every listed feature is already present in the cloned repository. Inspect the code and mark each feature as **implemented**, **in progress**, or **planned** as you work.
