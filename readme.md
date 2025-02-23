# Social Media Application called "Chattr"

========================================

Chattr is a social media application that allows users to create posts and share them with other users. Users can also comment on posts and like posts.

## Features

- Create posts
- Share posts
- Comment on posts
- Like posts

## Technologies used

- React
- NodeJS + ExpressJS
- MongoDB

## Setup Instructions

1. Database setup
   (If Local DB is used)
   - Install MongoDB Community Server from https://www.mongodb.com/try/download/community
   - Install MongoDB Compass from https://www.mongodb.com/docs/compass/current/install/
   - Create a new database called `chattr`
   - Create a new collection called `users`
   - Create a new collection called `posts`
   - Create a new collection called `comments`
   - Create a new collection called `likes`

(If Atlas DB is used)

- Visit https://www.mongodb.com/cloud/atlas
- Create a new cluster
- Create a new database called `chattr`
- Create a new collection called `users`
- Create a new collection called `posts`
- Create a new collection called `comments`
- Create a new collection called `likes`

2. Server setup

   - Create a new repository called "be-chattr"
   - Initialize a new NodeJS project

   To initialize package.json file without any prompts, run the following command:

   ```bash
    npm init -y
   ```

   or

   To initialize package.json file with prompts, run the following command:

   ```bash
   npm init
   ```

   - Install the following dependencies:

     - express
     - mongoose
     - cors
     - dotenv
     - nodemon (dev dependency)
     - morgan (dev dependency)
     - jsonwebtoken
     - bcrypt
     - multer

   - To install the dependencies, run the following command:

   ```bash
   npm install express mongoose cors dotenv jsonwebtoken bcrypt multer
   ```

   - To install the dev dependencies, run the following command:

   ```bash
   npm install nodemon morgan --save-dev
   ```

   - Create a new file called `.env` and add the following environment variables:

   ```bash
   PORT=3001
   MONGODB_URI=mongodb://localhost:27017/chattr
   JWT_SECRET=secret
   ```

   - Create a new file called `server.js`
     - Database connection setup
     - Express server setup
     - Middleware setup - cors, express.json, morgan, authentication
     - Routes setup
     - Controller setup
     - Model setup
     - Error handling setup
   - Following the MVC architecture, create the following folders:

     - controllers
     - models
     - routes

3. Client setup

   - Create a new repository called "fe-chattr"
   - Initialize a new React project

   To create a new React project, run the following command:

   ```bash
   npm create vite@latest fe-chattr
   ```

   - Install the following dependencies:

     - react-router-dom
     - axios
     - react-icons
     - react-toastify
     - tailwindcss
     - @headlessui/react
     - @heroicons/react

   - To install the dependencies, run the following command:

   ```bash
   npm install react-router-dom axios react-icons react-toastify tailwindcss @headlessui/react @heroicons/react
   ```
