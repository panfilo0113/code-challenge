# Challenge 3: Full Stack (Laravel) Development

In this challenge, you will create a full-stack web application using the Laravel PHP framework and, optionally, React for the frontend. Your application should implement a library management system with the following features:

## Backend Requirements

1. Create a Laravel application with a backend API to manage the books in the library. The API should provide endpoints to perform CRUD operations on the books, such as adding a book, deleting a book, updating a book, and retrieving a book by ID.

2. Implement a `Book` model with the following properties:
    - `id`: A unique identifier for the book.
    - `title`: The title of the book.
    - `author`: The author of the book.
    - `publisher`: The publisher of the book.
    - `publication_date`: The publication date of the book in `YYYY-MM-DD` format.
    - `isbn`: The ISBN number of the book.
    - `price`: The price of the book.
    - `genre`: The genre of the book.
    - `quantity`: The number of copies of the book available in the library.

   Use Eloquent ORM to interact with the database.

3. Use Laravel migrations to create a database schema for storing the book data.

4. Use Laravel API resources to transform the book data returned by the API endpoints.

5. Write a script to import the data from `books.json` into the Laravel backend/database.

## Frontend Requirements

1. Implement a frontend that consumes the Laravel API. This frontend should allow users to view the list of books, add new books, search and filter books. You can choose how you approach this, you can either implement standard Laravel MVC using Blade templates, or you can create a separate frontend application using Next.js or similar.

2. Display the list of books in a grid format (3 to 5 books per row). Please refer to the following [Figma Mockup](https://www.figma.com/file/9jMci6xwgORWWgAEBeXTnl/BookzRUs-Mockup?node-id=0%3A1&t=W4BIRXDOoLRu3oFM-1) as a reference.

3. Display the cover image for each book, retrieved from the Open Library Covers API or Google Books API.

4. If a book cover image is not available, display a fallback image.

5. Allow users to filter the list of books by genre.

6. Sort the list of books by title or author in ascending or descending order.

7. Allow users to click on a book to view more details on a separate book detail page.

## Optional Frontend Requirements

1. Implement the frontend using React and CSS Modules. You may have chosen to use Next.js for the frontend or perhaps you prefer to use Blade templates but integrate React components for some of interactive elements. Either approach is fine.

2. Make the CSS responsive for optimized display on different screen sizes.

3. Implement pagination to display the books in smaller chunks (e.g., 5 or 10 per page).

4. Add a search bar that allows users to search for books by title, author, or publisher.

5. Advanced: Create a feature to allow visitors to add books to a wishlist for later.

6. Advanced: Implement unit tests for your code.
