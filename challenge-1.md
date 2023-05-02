# Challenge 1: PHP Development

Implement a `Book` class that will represent a book in a library application. The `Book` class should have the following properties:

- `id`: A unique identifier for the book.
- `title`: The title of the book.
- `author`: The author of the book.
- `publisher`: The publisher of the book.
- `publication_date`: The publication date of the book in `YYYY-MM-DD` format.
- `isbn`: The ISBN number of the book.
- `price`: The price of the book.
- `genre`: The genre of the book.
- `quantity`: The number of copies of the book available in the library.

Your task is to implement the `Book` class with the above properties, and also implement the following methods:

- `findAll()`: This method should return an array of all books in the library.
- `findById($id)`: This method should return the book with the given ID, or `null` if no such book exists.
- `findByGenre($genre)`: This method should return an array of books that belong to the given genre.

You can assume that the book data is stored in a JSON file located at `data/books.json`. You should load this file and use it to initialize your `Book` objects.

**Note**: You can assume that the JSON file contains an array of book objects, where each book object has the following properties:

_See `data/books.json` for a sample file you can use as a starting point._

## Optional: Advanced Sorting, Filtering and Testing

If you're looking for an additional challenge and want to earn bonus points, you can attempt one or more of the following optional advanced tasks for this challenge:

1. Create a new class method in the `Book` class that sorts the list of books by title or author in ascending or descending order. The method should take two parameters: the field to sort by (`title` or `author`) and the order (`asc` or `desc`).

2. Create a new class method in the `Book` class that filters the list of books by genre. The method should take one parameter: the genre to filter by. It should return a list of books that match the given genre.

3. Create a new class method in the `Book` class that filters the list of books by publication year. The method should take one parameter: the year to filter by. It should return a list of books that were published in the given year.

4. Modify the `findAll` method to allow filtering and sorting by genre and publication year. The method should take two optional parameters: the genre to filter by and the year to filter by. If these parameters are provided, the method should return only the books that match the given criteria, sorted by title or author in ascending or descending order.

5. Add appropriate error handling for any invalid parameters or queries.

6. Advanced: Create a new class method in the `Book` class that calculates the average price of books in a given genre.

7. Advanced: Create a new class method in the `Book` class that calculates the total quantity of books in stock.

8. Advanced: Implement unit tests for your `Book` class to ensure that it works as expected.

_Note: You can still use the provided JSON data for the advanced portion of this challenge._
