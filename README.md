MERN Stack To-Do Application

A simple To-Do application built using the MERN stack (MongoDB, Express, React, Node.js). This application allows users to add, edit, delete, and mark tasks as complete or incomplete.

Features

Add, edit, and delete tasks.

Mark tasks as complete or incomplete.

Data is stored in MongoDB.

Full-stack application with both frontend and backend in a single repository.

Tech Stack

Frontend: React

Backend: Node.js, Express

Database: MongoDB

Getting Started

Prerequisites

Node.js installed on your machine.

A MongoDB account or a locally running MongoDB instance.

Installation

Clone the Repository:

bash

Copy code

git clone https://github.com/JaiKumar1003/cultureLinkr-todoListApp.git

cd todo-app

Install Dependencies: Install both frontend and backend dependencies.

bash

Copy code

cd client

npm install

cd ../server

npm install

Configuration

MongoDB Setup:

Create a .env file in the server directory with the following variables:

plaintext

Copy code

MONGO_URI=mongodb://localhost:27017/

PORT=5000

Proxy Setup for Development:

In the client package's package.json file, add the following line to set up a proxy to the backend for development:

json

Copy code

"proxy": "http://localhost:5000"

Running the Application

Start the Backend Server:

Open a terminal in the server directory and run:
bash
Copy code
npm start
This will start the Express server on http://localhost:5000.
Start the Frontend Server:

Open another terminal in the client directory and run:
bash
Copy code
npm start
This will start the React development server on http://localhost:3000.
Access the Application:

Open http://localhost:3000 in your browser to use the To-Do application.

Push to GitHub:

Make sure all your changes are committed and push the code to your GitHub repository.

API Endpoints

Method	Endpoint	Description

GET	/tasks	Get all tasks

POST	/tasks	Add a new task

PATCH	/tasks/:id/toggle	Toggle task completion

PUT	/tasks/:id	Update a task's title

DELETE	/tasks/:id	Delete a task

Usage

Add Task: Enter a title in the input field and click "Add Task".

Edit Task: Click the "Edit" button next to a task to modify its title.

Delete Task: Click "Delete" to remove a task.

Toggle Complete: Check the box next to a task to mark it as complete or incomplete.
