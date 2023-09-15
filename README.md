# Album Archive Project
For this project, I decoupled one of my previous projects to serve as the API for my frontend. The API is used to log user info as well as their own collection of music albums, whereas the frontend serves as a way for users to navigate and record their info. Users go to the webpage, createa user to login, and start a record of what they have from their personal collection. You can see a visual representation by navigating to the Github Projects link attached to this repository, or by clicking this link here: [Github Project](https://github.com/users/MoHanSolo/projects/3/views/1).

## Global Installation 

- Must install a couple of packages globally. This means you are allowed to use the code in the package on your local computer:

- [Node.js](https://nodejs.org/en)

Node.js is a cross-platform JavaScript runtime environment

- [MongoDB](https://www.mongodb.com/)

MongdoDB is a document database used to build scalable internet applications

- [Nodemon](https://nodemon.io/)

Nodemon is a Command-line tool that helps development for Node.js apps

## Installation Guide

Welcome to the installation portion for the Album's API! Here, I give a step-by-step walkthrough on how to install and get the API running. If you're a seasoned software engineer or just starting out, this guide should be simple enough for you to follow along.

First things first, we must clone the repository from Github into an empty repository on your computer.

1. After confirming you're on the necessary Github repository page, navigate to the "Code" button at the top in green. Click on the button. You should be under the local tab, if not click on it. We'll only be dealing with the SSH link provided. Make sure you copy the link and open up your terminal. I use GitBash since i'm using a Windows OS. 
2. Now were at the terminal, make sure you either create then navigate to the newly created folder or just navigate to the folder you wish to clone the repository in.
3. Initialize the repository by typing the following in the command line:

     `git init`

4. You should still have the copied SSH from Github, if not go back to the website and copy it. Once copied, paste it into the command line, it should look something like this:

    `git clone git@github.com:user/sampleAPI.git`

5. On your machine's command line, navigate to the folder you initialized and cloned the repo to by inputing the following:

    `cd folder-example`

    - Now that you're here, run the following:

    `npm i`

    - This installs all the necessary packages to get the API up and running

    - Next, we're going to create a .env file. Run this commmand to do so:

    `touch .env`
    
    - Now that everythings installed, we're ready to open up the API in our text editor of choice, i'm preferential to VSCode. You can do this by running the following, 

    `code .`

6. Now that we've opened up the project, we can navigate to our .env file. 

    - In here, we are going to add our MongoDB connection string (replace with your info):

    `PORT=3000
     SECRET_KEY=secret

     MONGO_URI=mongodb+srv://username:<password>@cluster.onedlis.mongodb.net/APIname?retryWrites=true&w=majority`


## Development Mode
- To run the application in development mode, simply run this command on the command line or within the command line of your preferred code editor: 

`npm run dev`

This will run the API in development mode, which allows you to make changes within the code while the server is still running. The server will automatically refresh the changes that have been made. 

## Starting the API
- To start the application, simply run this command on the command line or within the command line of your preferred code editor:

`npm start`

## API Requests via Postman

Now that our API is up and running, we must now open up [Postman](https://www.postman.com/). You can use the web version, but I highly suggest downloading it.

## Technology used for Albums API

- Node.js
- Express.js
- MongoDB
- Mongoose
- Nodemon
- bcrypt
- jsonwebtoken
- Mongodb-memory-server