# Challenge 2: Frontend (HTML/CSS & JS)

For this challenge, you are required to create a frontend web page that displays the list of books from the JSON file provided in Challenge 1. The web page should meet the following requirements:

- Display the list of books in a grid format (3 to 5 books per row).
- Use semantic HTML to structure the content.
- Display the cover image for each book, (you can retrieve covers from the Open Library Covers API or Google Books API.
- If a book cover image is not available, display a fallback image.
- Allow users to filter the list of books by genre.
- Sort the list of books by title or author in ascending or descending order.
- Allow users to click on a book to view more details on a separate book detail page.

You may use a frontend library or framework of your choice, such as React, to help with presentation. However, the logic should be implemented using your own custom code (e.g. don't integrate additional libraries that handles the filtering use standard js or standard React api's). The CSS styling should be done yourself without relying on frameworks or libraries like Bootstrap or Tailwind, you can use either css or scss.

To retrieve the cover images for the books, you can use the Open Library Covers API or Google Books API. Both APIs provide book cover images that can be accessed using the book's ISBN or identifier.

1) Open Library Covers API: This API provides a simple way to get cover images for books given their ISBN-10 or ISBN-13. To use it, you can make a GET request to the following URL: https://covers.openlibrary.org/b/isbn/{ISBN}-L.jpg, where {ISBN} is replaced by the book's ISBN-10 or ISBN-13. The "L" in the URL specifies the size of the image (large), but other options are available, such as "M" (medium) and "S" (small).

2) Google Books API: This API provides cover images as well as other book information, such as author, publisher, and summary. To use it, you can make a GET request to the following URL: https://www.googleapis.com/books/v1/volumes?q={search term}, where {search term} is replaced by the book's title or ISBN-10. The response includes an array of items, each representing a book, and the cover image can be found in the "imageLinks" object under "thumbnail".

Use only one of these services, if the cover image is not available then display a fallback image.

## Optional: Advanced Frontend Functionality

If you're up for an additional challenge to earn some bonus points you may like to attempt 1 or more of the following optional advanced challenges:

1. Make the CSS responsive for optimised display on different screen sizes

2. Implement pagination to display the books in smaller chunks (e.g. 5 or 10 per page).

3. Implement the frontend using Next.js

4. Use the Open Library API or Google Books API to obtain additional details to obtain additional information to display on the detail page.

5. Allow users to sort books by publication date.

6. Add a search bar that allows users to search for books by title, author, or publisher.

7. Advanced: Create a feature to allow visitors to add books to a wishlist for later.

8. Advanced: Implement unit tests for your frontend code.
