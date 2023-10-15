# Instagram Backend API

This project represents a basic design for the backend of an Instagram-like application. It provides functionality for user authentication and managing user posts.

## Endpoints

### User Controller

#### Sign In
- **Endpoint:** `POST /api/user/signin`
- **Description:** Sign in with a registered user account.
- **Request Body:**
  ```json
  {
    "email": "user@example.com",
    "password": "your_password"
  }
## Response:
 # Returns an authentication token on successful sign-in.

 
### Sign Up
- Endpoint: POST /api/user/signup 
- Description: Create a new user account.
- **Request Body:**
  ```json {
  "firstName": "John",
  "lastName": "Doe",
  "email": "newuser@example.com",
  "password": "your_password",
  "age": 25,
  "phoneNumber": "123-456-7890"
}

## Response:
# Returns a success message on successful sign-up.

# Update User Details
- Endpoint: PUT /api/user/{userId}
- Description: Update user details.
- **Request Body:**
  ```json {
  "firstName": "UpdatedFirstName",
  "lastName": "UpdatedLastName",
  "age": 30,
  "phoneNumber": "987-654-3210"
}

## Response:
# Returns the updated user object.
- Post Controller
- Save Post
#### Endpoint: POST /api/post
#### Description: Create a new post.
- **Request Body:**
  ```json {
  "postData": "Your post content here"
}

### Response:
- Returns the created post.
- Get Post
- Endpoint: GET /api/post/{postId}
- Description: Retrieve a post by its ID.
## Response:
- Returns the requested post.
## Usage
- Start the application.
- Use an API testing tool such as Postman to interact with the API.
- Sign in, sign up, create posts, and retrieve posts using the provided endpoints.
### Installation
- Clone the repository.
- Set up a database and configure the database connection in the application properties.
- Build and run the application.
- Dependencies
- Java
- Spring Boot
- Spring Data JPA
- Spring Security
- H2 Database (for testing, you can replace it with your preferred database)

### License
## This project is licensed under the MIT License - see the LICENSE.md file for details.

