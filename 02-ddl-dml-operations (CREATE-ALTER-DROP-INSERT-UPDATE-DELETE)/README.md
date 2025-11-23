# DDL & DML Operations (CREATE ALTER DROP INSERT UPDATE DELETE)

## ⭐ Task 01 — Create a table for storing books with the following columns: book_id, title, title, author, published_year, price

**Solution**

```sql
CREATE TABLE book_storage(
	book_id INT NOT NULL,
	title VARCHAR(150) NOT NULL,
	author VARCHAR(100) NOT NULL,
	published_year INT,
	price DECIMAL(10,2)
	CONSTRAINT pk_storage PRIMARY KEY (book_id)
)

SELECT *
FROM book_storage
```

**Result**

![exercise01](files-and-screenshots/01.Exercise_results.jpg)

## ⭐ Task 02 — Delete "published_year" column and add new column "year_of_publish"

**Solution**

```sql
ALTER TABLE book_storage
DROP COLUMN published_year

ALTER TABLE book_storage
ADD year_of_publish INT 

SELECT *
FROM book_storage
```

**Result**

![exercise01](files-and-screenshots/02.Exercise_results.jpg)
