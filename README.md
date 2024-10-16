# Product-Details

# Overview
This project is a full-stack application that allows users to view, search, select, and delete products. It consists of a Node.js backend (Express) to fetch product data from an external API and a React frontend that displays this data with features like search (with custom debouncing), pagination, row selection, and deletion (in memory).

# System Requirements
Ensure the following tools are installed on your machine:
1. 	Node.js (version 14 or higher)
 	  Download Node.js
2. 	npm (comes bundled with Node.js)

# Project Setup
1. Clone the Repository
First, clone the project repository (or download the files):
  git clone https://github.com/your-repository-link.git
Alternatively, you can download the project ZIP file and extract it.

2. Navigate into the Project Directory
Use the terminal or command prompt to navigate into the project directory:
  cd trika-challenge

# Backend (Node.js) Setup
1. Install Dependencies for the Backend
The backend is located in the root of the trika-challenge directory. You need to install all necessary dependencies:
npm install
This will install the following packages:
  express: Web framework for building the API server.
  axios: Used to fetch data from the external API.
  cors: Middleware to enable cross-origin resource sharing between frontend and backend.

2. Running the Node.js Backend
To start the Node.js backend server, use the following command:
  node server.js
The backend will now be running on http://localhost:3001 and will serve product data when the /products endpoint is accessed.

# Frontend (React) Setup
1. Navigate to the Frontend Directory
Change into the React frontend folder if you haven't already:
cd Frontend\trika-frontend

3. Install Dependencies for the Frontend
Install the necessary packages for the React app by running:
  npm install
This will install:
  axios: For making HTTP requests to the Node.js server to fetch product data.

4. Running the React Frontend
Start the frontend development server with:
  npm start
The React app will now run on http://localhost:3000. You can access the app through your browser.

# Running the Full Application
Once both the backend and frontend servers are running:
Backend will be running at http://localhost:3001/products (Node.js).
Frontend will be accessible via http://localhost:3000 (React).
 
# Key Features
1. Search with Debouncing: Users can search products, and the filtering only happens when they stop typing for 300ms to optimize performance.
2. Pagination: The app displays 10 products per page. Navigation buttons are available to switch between pages.
3. Row Selection: Users can select individual rows or use a "Select All" option for the visible rows.
4. In-Memory Deletion: Users can delete rows, and the data is only removed locally without affecting the backend.
 

