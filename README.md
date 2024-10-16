# Product-Details

# Overview
This project allows users to view, search, select, and delete products. It consists of a Node.js backend to fetch product data from an external API and a React frontend that displays this data with features like search (with custom debouncing), pagination, row selection, and deletion (in memory).

# System Requirements
Ensure the following tools are installed on your machine:
1. 	Node.js (version 14 or higher)
 	  Download Node.js
2. 	npm (comes bundled with Node.js)

# Project Setup<br>
1. Clone the Repository<br>
First, clone the project repository (or download the files):<br>
  git clone https://github.com/your-repository-link.git<br>
Alternatively, you can download the project ZIP file and extract it.

2. Navigate into the Project Directory
Use the terminal or command prompt to navigate into the project directory:
  cd trika-challenge

# Backend (Node.js) Setup
1. Install Dependencies for the Backend: <br>
The backend is located in the root of the trika-challenge directory. You need to install all necessary dependencies:<br>
 npm install<br>
This will install the following packages:<br>
* express: Web framework for building the API server.
* axios: Used to fetch data from the external API.
* cors: Middleware to enable cross-origin resource sharing between frontend and backend.

2. Running the Node.js Backend:<br>
   To start the Node.js backend server, navigate to Backend folder and use the followin command:<br>
      node server.js<br>
   The backend will now be running on http://localhost:3001 and will serve product data when the /products endpoint is accessed.

# Frontend (React) Setup
1. Navigate to the Frontend Directory<br>
Change into the React frontend folder:<br>
cd Frontend\trika-frontend<br>

3. Install Dependencies for the Frontend<br>
Install the necessary packages for the React app by running:<br>
  npm install<br>
This will install:<br>
  axios: For making HTTP requests to the Node.js server to fetch product data.

4. Running the React Frontend<br>
Start the frontend development server with:<br>
  npm start<br>
The React app will now run on http://localhost:3000. You can access the app through your browser.<br>

# Running the Full Application
Once both the backend and frontend servers are running:<br>
* Backend will be running at http://localhost:3001/products (Node.js).
* Frontend will be accessible via http://localhost:3000 (React).
 
# Key Features
1. Search with Debouncing: Users can search products, and the filtering only happens when they stop typing for 300ms to optimize performance.
2. Pagination: The app displays 10 products per page. Navigation buttons are available to switch between pages.
3. Row Selection: Users can select individual rows or use a "Select All" option for the visible rows.
4. In-Memory Deletion: Users can delete rows, and the data is only removed locally without affecting the backend.
 

