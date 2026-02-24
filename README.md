# Book-Sales-Data-Warehouse-MySQL

##  Project Overview

This project demonstrates a Data Warehouse built using MySQL.
The design follows a **Star Schema** model with one Fact table and multiple Dimension tables.

##  Data Model

### Fact Table
- fact_book_sales

### Dimension Tables
- dim_authors
- dim_publishers
- dim_formats
- genre

 ##  Database Schema (DDL)

## 1. dim_Author Foreign Key
 
 ```sql
ALTER TABLE fact_book_sales
ADD CONSTRAINT fk_author_id
FOREIGN KEY (author_id) REFERENCES dim_authors(author_id);
 ```
## 2. dim_publishers Foreign Key

 ```sql
ALTER TABLE fact_book_sales
ADD CONSTRAINT fk_publisher_id
FOREIGN KEY (Publisher_id) REFERENCES dim_publishers(publisher_id);
 ```
## 3. dim_formats Foreign key

 ```sql
ALTER TABLE fact_book_sales
ADD CONSTRAINT fk_format_id
FOREIGN KEY (format_id) REFERENCES dim_formats(format_id);
 ```
## 4. genre Foreign Key

```sql
ALTER TABLE fact_book_sales
ADD CONSTRAINT fk_genre_id
FOREIGN KEY (genre_id) REFERENCES genre(genre_id);
```

##  Skills Demonstrated
- Data Modeling
- Star Schema Design
- Fact & Dimension Tables
- Foreign Key Relationships


















  
