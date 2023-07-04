# User Self Management Endpoints

This endpoints

## Login

Authenticates a user and set admin and token cookies.

-   Method: POST
-   Endpoint: `/login`
- admin level: `0`
-   Required Parameters:
    -   `username`: User's username
    -   `password`: User's password

## Update User Properties

Updates the user's profile information.

-   Method: PATCH
-   Endpoint: `/user_properties_change`
- admin level: `0`
-   Optional Parameters:
    -   `username`: New username
    -   `email`: new email
    -   `passw`: new password

## Register New User

Registers a new user in the application.

-   Method: POST
-   Endpoint: `/register`
- admin level: `0`
-   Required Parameters:
    -   `username`: User's desired username
    -   `email`: User's email address
    -   `password`: User's desired password
