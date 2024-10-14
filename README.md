# The Growth Hub
A full-stack web application that allows users to create, edit, view, and delete blog posts. The project is built using Node.js, Express, EJS, and Axios, with a custom API developed by me.

## Features
* Create a new blog post
* Edit an existing blog post
* Delete blog posts
* View all blog posts in a list with details such as title, content, author, and date
* Responsive and dynamic UI with EJS templates for the frontend
* API-based interaction between the backend and the frontend using Axios
  
### Project Structure
The project is divided into two main parts:
1. API (API Responds port:4000)

* Manages the posts (in-memory store)
* Provides CRUD operations for blog posts
* Custom API built by me using Node.js and Express
  
2. Backend (Makes API requests port:3000)

* Displays blog posts to users
* Offers UI for creating, editing, and deleting posts
* Communicates with the backend API to manage data

### API 
The API is custom-built using Node.js and Express and handles all operations related to managing blog posts. The API provides the following routes:

* GET /posts – Fetch all posts
* GET /posts/:id – Fetch a specific post by its ID
* POST /posts – Create a new post
* PATCH /posts/:id – Update an existing post
* DELETE /posts/:id – Delete a post
  
### Backend
The backend uses EJS templates to render the blog posts. Axios is used to make API requests to the backend server. The application has the following routes:

* / – Main page to view all posts
* /new – Create a new post
* /edit/:id – Edit an existing post
* /about – About page (static)
  
Installation
Prerequisites
Make sure you have the following installed:

Node.js (version 14 or higher)
npm (comes with Node.js)

Clone the Repository
```
git clone https://github.com/your-username/blog-post-manager.git
cd <to the file>
```
Install Dependencies
```
npm install
```
Run the Application
There are two separate servers for the backend and the API.

Start the backend API server:
```
node index.js
```
This starts the API at http://localhost:4000.

Start the backend server:
```
node server.js
```
This starts the backend application at http://localhost:3000.
Make sure both servers run at the same time for the website to work.

#### Testing the Application
* Go to http://localhost:3000 to view the blog posts.
* Click on "New Post" to add a new blog entry.
* Click on the edit or delete icons to modify or remove posts.
