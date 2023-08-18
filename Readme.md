
# Project Instagram - User Management System

Welcome to the documentation for the Instagram-like user management system project. This guide provides an overview of the project structure and functionality.

## Table of Contents

- [Introduction](#introduction)
- [Client-side](#client-side)
  - [Login](#login)
  - [Register](#register)
  - [User Page](#user-page)
- [Server-side](#server-side)
  - [Database Setup](#database-setup)
  - [User Routes](#user-routes)
  - [Middleware](#middleware)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project aims to create a user management system similar to Instagram. It allows users to sign up, log in, and view their profile details.

## Client-side

### Login

The login page (`Login.html`) provides a form for users to enter their username and password. Upon submission, the form triggers an API call to the server for user authentication.

### Register

The registration page (`Register.html`) allows users to create an account by providing their name, email, password, bio, and username. After submitting the form, an API call is made to the server for user registration.

### User Page

The user page (`index.html`) displays user details, including the profile image, username, bio, email, and follower count. The user's data is fetched from the server using an API call.

## Server-side

### Database Setup

The `db.js` file configures the connection to the MongoDB database using Mongoose.

### User Routes

The `user.route.js` file contains routes related to user functionality, such as signing up, logging in, and fetching user details.

### Middleware

- `authenticateUser.js`: This middleware verifies the user's authentication by checking the presence and validity of a JWT token.

- `signup.validator.js`: This middleware validates the input fields during user registration.

- `login.validator.js`: This middleware validates the input fields during user login.

### User Controller

The `user.controller.js` file includes functions to handle user-related operations such as signing up, logging in, and fetching user details. It also uses bcrypt for password hashing and JWT for token generation.

## Usage

1. Install the required dependencies for both the client and server using `npm install`.
2. Configure the MongoDB connection by adding the database URL to the `.env` file.
3. Run the server using `npm start` in the `Server` directory.
4. Open the client files (`Login.html`, `Register.html`, `index.html`) in a browser to interact with the application.

## Contributing

Contributions are welcome! Feel free to submit pull requests to improve the code or add new features.

## License

This project is licensed under the [ISC License](LICENSE).

---

Please note that this is a high-level overview. You might want to add more details, deployment instructions, and any other relevant information to the documentation as needed.
