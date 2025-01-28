# JSONPlaceholder API Testing with Postman

This repository contains a collection of **JSONPlaceholder API requests** created for practicing API testing in **Postman**. It includes various CRUD operations with validations such as status code checks, response validation, and more.

---

## Table of Contents

- [About JSONPlaceholder](#about-jsonplaceholder)
- [Project Features](#project-features)
- [Requests Covered](#requests-covered)
- [Validations Applied](#validations-applied)
- [Getting Started](#getting-started)
- [How to Use](#how-to-use)
- [Postman Collection](#postman-collection)


---

## About JSONPlaceholder

JSONPlaceholder is a free online REST API for testing and prototyping. It provides mock endpoints that mimic real-world API interactions, making it ideal for learning and practicing API testing.

Official site: [JSONPlaceholder](https://jsonplaceholder.typicode.com/)

---

## Project Features

- Implemented **CRUD operations** for testing APIs.
- Requests include:
  - Fetching data (GET)
  - Creating new data (POST)
  - Updating data (PUT/PATCH)
  - Deleting data (DELETE)
- Added **validation tests** for:
  - HTTP status codes
  - Response structure and content

---

## Requests Covered

1. **Get All Posts**  
   Endpoint: `GET /posts`  
   Description: Retrieves a list of all posts.

2. **Get Specific Post by ID**  
   Endpoint: `GET /posts/{id}`  
   Description: Retrieves a post using its unique ID.

3. **Create a Post**  
   Endpoint: `POST /posts`  
   Description: Adds a new post with a custom payload.

4. **Update a Post**  
   - Full Update: `PUT /posts/{id}`  
   - Partial Update: `PATCH /posts/{id}`  
   Description: Updates a specific post entirely or partially.

5. **Delete a Post**  
   Endpoint: `DELETE /posts/{id}`  
   Description: Deletes a specific post using its ID.

---

## Validations Applied

For each request, the following validations have been added:

1. **Status Code Validation** 
   - Ensures the response status code is as expected.  
     Example: `200 OK` for GET, `201 Created` for POST, etc.

2. **Response Body Validation**  
   - Validates the structure and content of the response body.  
     Example: Ensures that required fields like `id`, `title`, and `body` exist in the response.


---

## Getting Started

### Prerequisites

- Install **Postman** for testing: [Download Postman](https://www.postman.com/downloads/)


## How to Use

Follow these steps to test the JSONPlaceholder API requests using the Postman collection:

1. **Clone the Repository**
   - Clone this repository to your local machine:
     ```bash
     git clone https://github.com/<your-username>/jsonplaceholder-api-testing.git
     ```
   - Navigate to the project folder:
     ```bash
     cd jsonplaceholder-api-testing
     ```

2. **Open Postman**
   - Ensure you have Postman installed. If not, [download it here](https://www.postman.com/downloads/).

3. **Import the Postman Collection**
   - Open Postman and click on the **"Import"** button in the top-left corner.
   - Select the file `JSONPlaceholder.postman_collection.json` from the repository folder.
   - The collection will appear in your Postman workspace.

4. **Run the Requests**
   - Expand the imported collection in Postman.
   - Each request (GET, POST, PUT, DELETE, etc.) is organized under relevant folders.
   - Click on any request to test the endpoint.
   - Add your input (e.g., body data for POST or PUT requests) where applicable.

5. **View and Edit Validations**
   - Go to the **"Tests"** tab for any request.
   - Review the prewritten test scripts, including status code and response validation.
   - Modify or add new validation scripts if needed.

---   

## Postman Collection

The **Postman Collection** includes all the necessary requests for testing JSONPlaceholder APIs, along with predefined validations.

### Download the Collection
- The collection file is included in this repository:  
  [JSONPlaceholder.postman_collection.json](./JSONPlaceholder.postman_collection.json)

### Collection Structure
The collection is organized as follows:

- **Posts**  
  - `GET /posts`: Fetch all posts.  
  - `GET /posts/{id}`: Fetch a specific post using its ID.  
  - `POST /posts`: Create a new post.  
  - `PUT /posts/{id}`: Update an existing post completely.  
  - `PATCH /posts/{id}`: Update specific fields of a post.  
  - `DELETE /posts/{id}`: Delete a specific post.
 
 ---

 With this collection, you can easily test and validate JSONPlaceholder APIs and practice working with RESTful APIs.
