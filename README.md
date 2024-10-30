# CS-312-MiniProject-4
# Blog Web Application Using React.js, Node.js, Express.js

## Objective
The objective of this mini-project is to enhance the basic blog web application created using Node.js, Express.js, and EJS. This project will enable users to create, view, edit, and delete blog posts. The previously used server-side rendering (EJS) will be replaced with a React.js frontend.

You can build this mini-project on top of Mini-Project-1 or Mini-Project-3. Integrating a database is optional, allowing for flexibility between database and no-database implementations.

## Instructions

### Step 1: Planning
- Gather content and design ideas. (Optional) Create wireframes and mockups.
- Plan out the database schemas and operations (structure, database interactions, etc.).

### Step 2: Setup
- Fork or clone the project repository for Mini-Project-3.
- Run the project using Node.js (ensure the database server is running) and verify that everything is working as expected.

### Step 3: Integrate React.js with the Backend
- Connect React.js with your Node.js backend.
- Define backend routes (e.g., GET, POST) to handle blog operations. Ensure responses are in JSON format.
- Use `fetch` or Axios in React to call Node.js backend endpoints (e.g., `http://localhost:8000/blogs`). Test with a simple API call and log the data in the console to confirm connection.

### Step 4: Signup and Sign in
- Create two React components: one for signing in and one for signing up.
- **Signup Page:** Form with inputs for `user_id`, `password`, `name`, and other details if needed.
- **Signin Page:** Form with inputs for `user_id` and `password`.
- On submission, pass credentials to the backend for authentication. Return success or error information to the frontend.

### Step 5: Post Creation
- Convert your existing EJS form for creating blog posts into a React component.
- Use state variables for form fields and bind them using the `value` attribute.
- Add a submit handler to process and submit the form data to the backend.

### Step 6: Post Viewing
- Create a React component, `PostList.js`, to dynamically render all posts on the homepage.
- Fetch posts from the backend and use the `.map()` method to display each post with title, content, and additional info.
- Include "Edit" and "Delete" buttons for each post.

### Step 7: Post Editing
- Implement an edit form in React that loads the existing post with pre-filled content fields.
- Ensure only the creator can edit their own posts by checking this in the backend.
- On submission, replace the original post with the updated version dynamically on the homepage.

### Step 8: Post Deletion
- When a user clicks the delete button for a post, send relevant information to the backend.
- If the user has necessary permissions, the blog should be deleted from the backend.
- Ensure deleted posts no longer appear on the homepage.

### Step 9: Styling
- Use CSS or a framework like Bootstrap to style your React application components.
- Ensure a responsive layout that looks good on both desktop and mobile devices.

### Step 10: Testing
- Test the application on different devices and browsers to ensure proper functionality.

## Bonus Challenge: (Optional)
### My Profile Section
- Create a "My Profile" section using a React component.
- Display all blogs posted by the user along with the user's information (e.g., username, name, age, occupation, etc.).
