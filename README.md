# Posts App

## Overview

Posts App is a full-stack application that allows users to create and view posts. The frontend is developed with React, while the backend is built using Node.js.

## Features

- **View All Posts**: Retrieve and display all posts.
- **View Single Post**: Retrieve and display a single post by its ID.
- **Create Post**: Add a new post to the collection.

## Frontend

The frontend is built using React and provides a user interface for interacting with the backend API.

### Features

- **Create Post**: Click the "New Post" button to open a form for creating a new post.
- **View All Posts**: All posts are displayed on the main page.

### Installation

1. Navigate to the frontend directory:
   ```bash
   cd frontend
2. Install the dependencies:
   ```bash
   npm install
3. Start the development server:
   ```bash
   npm run dev
   
### Usage

- Open the application in your browser at http://localhost:3000.
- Click the "New Post" button to create a new post.
- View all posts on the main page.

## Backend

The backend of this application is built using Node.js and provides the following API routes:

- **`GET /posts`**: Fetch all posts.
- **`GET /posts/:id`**: Fetch a single post by its ID.
- **`POST /posts`**: Create a new post.

### Installation

1. Navigate to the backend directory:
   ```bash
   cd backend
2. Install the dependencies:
   ```bash
   npm install
3. Start the server:
   ```bash
   npm start

### API Routes

- Fetch All Posts
  ```bash
  GET /posts
  
  Response:
   {
     "posts": [
       {
         "body": "Sample body 1",
         "author": "Author 1",
         "id": "1"
       },
       {
         "body": "Sample body 2",
         "author": "Author 2",
         "id": "2"
       },
       {
         "body": "Sample body 3",
         "author": "Author 3",
         "id": "3"
       }
     ]
   }

- Fetch Single Post
  ```bash
  GET /posts/:id
  
  Response:
   {
    "body": "Sample body",
    "author": "Sample author",
    "id": "1"
  }

- Create Post
  ```bash
  POST /posts
  
  Request Body:
   {
    "body": "Post content",
    "author": "Post author"
  }
  
  Response:
   {
    "body": "Post content",
    "author": "Post author",
    "id": "generated_id"
  }

## Frontend

The frontend is built using React and provides a user interface for interacting with the backend API.
