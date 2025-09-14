# Blogging-Platform-API
- https://roadmap.sh/projects/blogging-platform-api
  
You are required to create a simple RESTful API with basic CRUD operations for a personal blogging platform. CRUD stands for Create, Read, Update, and Delete.

## Goals

The goals of this project are to help you:

- Understand what the RESTful APIs are including best practices and conventions

- Learn how to create a RESTful API

- Learn about common HTTP methods like GET, POST, PUT, PATCH, DELETE

- Learn about status codes and error handling in APIs

- Learn how to perform CRUD operations using an API

- Learn how to work with databases

## Requirements

You should create a RESTful API for a personal blogging platform. The API should allow users to perform the following operations:

- Create a new blog post

- Update an existing blog post

- Delete an existing blog post

- Get a single blog post

- Get all blog posts

- Filter blog posts by a search term

### Create Blog Post

- Create a new blog post using the POST method

POST /posts
```
{
  "title": "My First Blog Post",
  "content": "This is the content of my first blog post.",
  "category": "Technology",
  "tags": ["Tech", "Programming"]
}
```
- Each blog post should have the following fields:

json
```
{
  "title": "My First Blog Post",
  "content": "This is the content of my first blog post.",
  "category": "Technology",
  "tags": ["Tech", "Programming"]
}
```

### Update Blog Post

- Update an existing blog post using the PUT method

PUT /posts/1
```
{
  "title": "My Updated Blog Post",
  "content": "This is the updated content of my first blog post.",
  "category": "Technology",
  "tags": ["Tech", "Programming"]
}
```
- The endpoint should validate the request body and return a 200 OK status code with the updated blog post.

json
```
{
  "id": 1,
  "title": "My Updated Blog Post",
  "content": "This is the updated content of my first blog post.",
  "category": "Technology",
  "tags": ["Tech", "Programming"],
  "createdAt": "2021-09-01T12:00:00Z",
  "updatedAt": "2021-09-01T12:30:00Z"
}
```
### Delete Blog Post

- Delete an existing blog post using the DELETE method
```
DELETE /posts/1
```

### Get All Blog Posts

- Get all blog posts using the GET method
```
GET /posts
```
