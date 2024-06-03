# Blog Project

## Description

This project is a simple blog application built using Node.js, Express, MongoDB, and EJS. It allows users to create, view, update and delete blog posts.

## Features

- View all blog posts
- Create new blog posts
- View details of a specific blog post
- Update snippet of a blog post
- Delete a blog post

## Technologies Used

- Node.js
- Express
- MongoDB
- Mongoose
- EJS
- Morgan

## Installation

1. *Clone the repository:*

   sh
   git clone <repository-url>
   cd <repository-directory>
   

2. *Install dependencies:*

   sh
   npm install
   

3. *Set up MongoDB:*

   Ensure you have a MongoDB database set up. Replace the connection string in the main file with your MongoDB connection string.

   js
   const dburl = "your-mongodb-connection-string";
   

4. *Run the application:*

   sh
   node app.js
   

   The server will start on http://localhost:3000.

## File Structure

- *app.js*: Main entry point of the application. Sets up the server, middleware, and routes.
- *routes/Blogroutes.js*: Contains the routes for the blog.
- *controllers/Blogcontroller.js*: Contains the logic for handling blog-related requests.
- *models/blog.js*: Defines the schema for blog posts.
- *views/*: Contains EJS files for rendering HTML pages.
- *public/*: Contains static files like CSS.

## Routes

- *GET /*: Display all blogs.
- *GET /create*: Render the form to create a new blog.
- *POST /blogs*: Create a new blog post.
- *GET /:id*: Get a specific blog post by ID.
- *POST /:id*: Update blog post snippet.
- *DELETE /:id*: Delete a blog post by ID.

## Middleware

- *morgan*: Logs HTTP requests.
- *express.static*: Serves static files from the public directory.
- *express.urlencoded*: Parses URL-encoded bodies.

## Views

The views are rendered using EJS. The following views are available:

- *index.ejs*: Home page displaying all blogs.

- *details.ejs*: Detailed view of a single blog post.

- *create.ejs*: Form to create a new blog post.

## Styles

The styles are located in the public folder. The main CSS file is styles.css.
