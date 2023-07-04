# /User Endpoint

The User endpoint allows you to manage user accounts in your application.

## Get Users

If `name ` isn't set retrieves a list of all users, if it's set it retrieves only the user matching the name.

- Method: GET
- Endpoint: `/user?name="user_name"`
-   admin level: `2`
- URL Parameters:
    - `name` (optional): User name 

## Create User

Creates a new user.

- Method: POST
- Endpoint: `/user`
-   admin level: `2`
- Required Parameters:
    - `name`: Name of the user
    - `email`: Email address of the user
    - `password`: Password for the user account

## Update User

Updates an existing user.

- Method: PATCH
- Endpoint: `/user`
-   admin level: `2`
- Required Parameters:
    - `id`: ID of the user to update
    - `name` (optional): New name for the user
    - `email` (optional): New email address for the user
    - `password` (optional): New password for the user account

## Delete User

Deletes a user.

- Method: DELETE
- Endpoint: `/user`
-   admin level: `2`
- Required Parameters:
    - `id`: ID of the user to delete
