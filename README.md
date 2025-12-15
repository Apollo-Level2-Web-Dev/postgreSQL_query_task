# Online Bookstore Database

## TABLE CREATION INSTRUCTIONS

### Instruction

Create the following three tables for an online bookstore database.  
Pay attention to data types, constraints, and relationships between tables.

---

### TABLE 1: customers

This table should store customer information with the following columns:

- `customer_id`: Integer, primary key
- `first_name`: Text field (max 50 characters)
- `last_name`: Text field (max 50 characters)
- `email`: Text field (max 100 characters)
- `city`: Text field (max 50 characters)
- `country`: Text field (max 50 characters)
- `registration_date`: Date field

---

### TABLE 2: books

This table should store book catalog information with the following columns:

- `book_id`: Integer, primary key
- `title`: Text field (max 200 characters)
- `author`: Text field (max 100 characters)
- `genre`: Text field (max 50 characters)
- `price`: Decimal number (10 digits total, 2 after decimal point)
- `publication_year`: Integer
- `stock_quantity`: Integer

---

### TABLE 3: orders

This table should store order information with the following columns:

- `order_id`: Integer, primary key
- `customer_id`: Integer that references the customers table
- `book_id`: Integer that references the books table
- `order_date`: Date field
- `quantity`: Integer
- `total_amount`: Decimal number (10 digits total, 2 after decimal point)

---

## DATASET TO INSERT

### Instruction

After creating your tables, insert the following data.  
You'll need to write INSERT statements for each table.

---

### CUSTOMERS DATA (10 records)

**Columns:** `customer_id`, `first_name`, `last_name`, `email`, `city`, `country`, `registration_date`

1. 1, John, Smith, john.smith@email.com, New York, USA, 2023-01-15
2. 2, Emma, Johnson, emma.j@email.com, London, UK, 2023-02-20
3. 3, Michael, Brown, mbrown@email.com, Toronto, Canada, 2023-01-10
4. 4, Sophia, Davis, sophia.d@email.com, Sydney, Australia, 2023-03-05
5. 5, James, Wilson, jwilson@email.com, New York, USA, 2023-02-28
6. 6, Oliver, Taylor, oliver.t@email.com, London, UK, 2023-04-12
7. 7, Ava, Anderson, ava.anderson@email.com, Los Angeles, USA, 2023-03-18
8. 8, William, Martinez, w.martinez@email.com, Madrid, Spain, 2023-01-25
9. 9, Isabella, Garcia, isabella.g@email.com, Mexico City, Mexico, 2023-02-14
10. 10, Lucas, Rodriguez, lucas.r@email.com, Buenos Aires, Argentina, 2023-03-30

---

### BOOKS DATA (14 records)

**Columns:** `book_id`, `title`, `author`, `genre`, `price`, `publication_year`, `stock_quantity`

1. 1, The Great Gatsby, F. Scott Fitzgerald, Fiction, 12.99, 1925, 45
2. 2, To Kill a Mockingbird, Harper Lee, Fiction, 14.99, 1960, 32
3. 3, 1984, George Orwell, Science Fiction, 13.99, 1949, 28
4. 4, Pride and Prejudice, Jane Austen, Romance, 11.99, 1813, 50
5. 5, The Catcher in the Rye, J.D. Salinger, Fiction, 12.99, 1951, 22
6. 6, Harry Potter and the Sorcerer Stone, J.K. Rowling, Fantasy, 19.99, 1997, 60
7. 7, The Hobbit, J.R.R. Tolkien, Fantasy, 15.99, 1937, 38
8. 8, Brave New World, Aldous Huxley, Science Fiction, 13.99, 1932, 25
9. 9, The Lord of the Rings, J.R.R. Tolkien, Fantasy, 29.99, 1954, 41
10. 10, Animal Farm, George Orwell, Fiction, 10.99, 1945, 55
11. 11, Fahrenheit 451, Ray Bradbury, Science Fiction, 12.99, 1953, 30
12. 12, The Great Adventure, John Anderson, Fiction, 16.99, 2020, 18
13. 13, Mystery in Paris, Marie Dubois, Mystery, 14.99, 2019, 27
14. 14, Romance in Rome, Isabella Rossi, Romance, 13.99, 2021, 35

---

### ORDERS DATA (18 records)

**Columns:** `order_id`, `customer_id`, `book_id`, `order_date`, `quantity`, `total_amount`

1. 1, 1, 1, 2023-05-10, 2, 25.98
2. 2, 1, 6, 2023-05-15, 1, 19.99
3. 3, 2, 3, 2023-05-12, 1, 13.99
4. 4, 3, 2, 2023-05-11, 3, 44.97
5. 5, 4, 7, 2023-05-13, 1, 15.99
6. 6, 5, 9, 2023-05-14, 2, 59.98
7. 7, 2, 4, 2023-05-16, 1, 11.99
8. 8, 6, 6, 2023-05-17, 2, 39.98
9. 9, 7, 1, 2023-05-18, 1, 12.99
10. 10, 8, 8, 2023-05-19, 1, 13.99
11. 11, 1, 10, 2023-06-01, 2, 21.98
12. 12, 3, 5, 2023-06-02, 1, 12.99
13. 13, 9, 11, 2023-06-03, 3, 38.97
14. 14, 10, 12, 2023-06-04, 1, 16.99
15. 15, 4, 13, 2023-06-05, 2, 29.98
16. 16, 5, 14, 2023-06-06, 1, 13.99
17. 17, 2, 6, 2023-06-07, 1, 19.99
18. 18, 7, 3, 2023-06-08, 2, 27.98

---

## PRACTICE QUESTIONS

1. Display all books with their titles and prices, ordered by price (lowest to highest)
2. Find all distinct countries where customers are from
3. Find all books whose titles start with `"The"`
4. Change the column name `first_name` to `customer_first_name` in the customers table
5. Find all books in the Fantasy genre
6. Count the total number of orders in the database
7. Find the average price of books by genre, but only show genres with an average price greater than `$14`
8. Find all customers whose email addresses end with `.com` and are from either USA or UK
9. Display all customers with their full name in **uppercase** (concatenated first and last name),  
   original email, and city in **lowercase**.  
   Only show customers from **USA** or **UK**.
10. Find the **total revenue**, **average order amount**, **maximum order amount**, and  
    **minimum order amount** from all orders placed in **June 2023**.
