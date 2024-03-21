# Book Management Application

This is a book management application that allows managing books, authors, and reviews. 

## Key Features

- Create, retrieve, update, and delete books
- Add and manage book reviews 
- Associate reviews with books and authors
- Manage book availability/inventory
- Add and manage authors
- Search/filter books by genre

## Code Overview

The core models are:

- Book 
- Author
- Review

The BookRepository contains key methods for:

- Creating, retrieving, updating and deleting books
- Managing book inventory/availability 
- Adding reviews to books and authors
- Getting books by genre
- Managing authors

## ROUTES ##
// Create a New Book 
POST /books

// Add Review to Target (Book or Author)
POST /books/:target/:targetId/reviews 

// Get Book Details by ID
GET /books/:bookId

// Update Book Availability 
PUT /books/:bookId

// Delete Book by ID
DELETE /books/:bookId

// List Books by Genre
GET /books/genre/:genre

// Create a New Author
POST /books/authors

// Associate an Author with a Book
POST /books/:bookId/authors

// List Authors of a Book
GET /books/:bookId/authors

// List Books by an Author
GET /books/authors/:authorId/books

## Running the App Locally

To run the app locally:

1. Clone the repository 
2. Install dependencies via npm: `npm install`
3. Configure your MongoDB connection string in `.env` 
4. Start the server: `npm run start`




