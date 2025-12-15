# Answers

## 1

| title                               | price |
| ----------------------------------- | ----- |
| Animal Farm                         | 10.99 |
| Pride and Prejudice                 | 11.99 |
| Fahrenheit 451                      | 12.99 |
| The Great Gatsby                    | 12.99 |
| The Catcher in the Rye              | 12.99 |
| Romance in Rome                     | 13.99 |
| 1984                                | 13.99 |
| Brave New World                     | 13.99 |
| Mystery in Paris                    | 14.99 |
| To Kill a Mockingbird               | 14.99 |
| The Hobbit                          | 15.99 |
| The Great Adventure                 | 16.99 |
| Harry Potter and the Sorcerer Stone | 19.99 |
| The Lord of the Rings               | 29.99 |

## 2

| country   |
| --------- |
| USA       |
| Canada    |
| Argentina |
| Australia |
| UK        |
| Spain     |
| Mexico    |

# 3

| book_id | title                  | author              | genre   | price | publication_year | stock_quantity |
| ------- | ---------------------- | ------------------- | ------- | ----- | ---------------- | -------------- |
| 1       | The Great Gatsby       | F. Scott Fitzgerald | Fiction | 12.99 | 1925             | 45             |
| 5       | The Catcher in the Rye | J.D. Salinger       | Fiction | 12.99 | 1951             | 22             |
| 7       | The Hobbit             | J.R.R. Tolkien      | Fantasy | 15.99 | 1937             | 38             |
| 9       | The Lord of the Rings  | J.R.R. Tolkien      | Fantasy | 29.99 | 1954             | 41             |
| 12      | The Great Adventure    | John Anderson       | Fiction | 16.99 | 2020             | 18             |

# 4

| Success. No rows returned |

- to verify run this query

```
SELECT * FROM customers LIMIT 1;

```

### revert back for continuing tests **customer_first_name** TO **first_name**

# 5

| book_id | title                               | author         | genre   | price | publication_year | stock_quantity |
| ------- | ----------------------------------- | -------------- | ------- | ----- | ---------------- | -------------- |
| 6       | Harry Potter and the Sorcerer Stone | J.K. Rowling   | Fantasy | 19.99 | 1997             | 60             |
| 7       | The Hobbit                          | J.R.R. Tolkien | Fantasy | 15.99 | 1937             | 38             |
| 9       | The Lord of the Rings               | J.R.R. Tolkien | Fantasy | 29.99 | 1954             | 41             |

# 6

| total_orders |
| ------------ |
| 18           |

# 7

| genre   | average_price |
| ------- | ------------- |
| Fantasy | 21.99         |
| Mystery | 14.99         |

# 8

| customer_id | first_name | last_name | email                  | city        | country | registration_date |
| ----------- | ---------- | --------- | ---------------------- | ----------- | ------- | ----------------- |
| 1           | John       | Smith     | john.smith@email.com   | New York    | USA     | 2023-01-15        |
| 2           | Emma       | Johnson   | emma.j@email.com       | London      | UK      | 2023-02-20        |
| 5           | James      | Wilson    | jwilson@email.com      | New York    | USA     | 2023-02-28        |
| 6           | Oliver     | Taylor    | oliver.t@email.com     | London      | UK      | 2023-04-12        |
| 7           | Ava        | Anderson  | ava.anderson@email.com | Los Angeles | USA     | 2023-03-18        |

# 9

| full_name     | email                  | city_lowercase |
| ------------- | ---------------------- | -------------- |
| AVA ANDERSON  | ava.anderson@email.com | los angeles    |
| EMMA JOHNSON  | emma.j@email.com       | london         |
| JAMES WILSON  | jwilson@email.com      | new york       |
| JOHN SMITH    | john.smith@email.com   | new york       |
| OLIVER TAYLOR | oliver.t@email.com     | london         |

# 10

| total_revenue | average_order_amount | maximum_order | minimum_order | total_orders_in_june |
| ------------- | -------------------- | ------------- | ------------- | -------------------- |
| 182.87        | 22.86                | 38.97         | 12.99         | 8                    |
