# Friends List Express Server

Welcome to the Friends List Express Server project! This lab will guide you through creating an application with API endpoints to perform Create, Retrieve, Update, and Delete operations on a Friends list using an Express server. The objective is to implement authentication at the session level using JSON Web Tokens (JWT) for authorized access.

## Project Overview

The Friends List Express Server allows you to manage a list of friends with their details such as First Name, Last Name, Email, and Date of Birth. You can add, retrieve, update, and delete friend details using the provided API endpoints.

## How to Get Started

To get started with the project, follow these steps:

1. Install the required packages by running `npm install` in the project directory.
2. Start the Express server by running `npm start`.
3. Test the endpoints using CURL or Postman.

## API Endpoints

The Express server provides the following API endpoints:

- **GET /user**: Retrieve the list of friends.
- **POST /user**: Add a new friend to the list.
- **PUT /user/:id**: Update the details of a specific friend.
- **DELETE /user/:id**: Delete a friend from the list.

Please note that `:id` in the URL represents the unique identifier of a friend.

## Authentication

Authentication is implemented at the session level using JSON Web Tokens (JWT). This ensures authorized access to the API endpoints. The necessary packages, such as `jsonwebtoken` and `express-session`, have been included in the project.

## Testing the Endpoints

To test the implemented endpoints, you can use cURL or Postman. Make requests to the respective endpoints with the appropriate HTTP methods (GET, POST, PUT, DELETE) to perform CRUD operations on the friend's list.

## Project Structure

The project directory structure is as follows:

- **routes/users.js**: Contains the endpoint handlers for the /user routes.
- **app.js**: Configures the Express server and sets up middleware.

Please refer to the provided code and comments within the files for further details and instructions.

Let's get started with managing your Friends list using the Friends List Express Server! Feel free to explore, modify, and enhance the project as per your requirements. If you have any questions or need assistance, feel free to reach out. Enjoy coding!
