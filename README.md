#  Hotel Database System (SQL + Database Design)

##  Overview
This project implements a **relational database system for hotel management**, designed to efficiently handle operations such as:

- Room management  
- Guest information   
- Reservations  
- Staff management   
- Payments   

The system is built using **SQL and database design principles**, ensuring structured storage, data integrity, and efficient querying.

> The database integrates multiple entities to support smooth hotel operations and enhance user experience :contentReference[oaicite:0]{index=0}.

---

##  Objectives

- Design a complete **Hotel Management Database**
- Create a normalized schema with relationships
- Implement tables using SQL
- Perform data insertion and querying
- Apply real-world database concepts

---

##  Database Design

###  Entity Relationship Diagram (ERD)

The system includes key entities:

- Hotel  
- Room  
- Guests  
- Staff  
- Reservation  
- Payment  

> The ERD (page 2) shows relationships between entities such as:
- Hotel → Rooms  
- Guests → Reservations  
- Staff → Services :contentReference[oaicite:1]{index=1}.

---

###  Database Schema

The schema defines tables with:
- Primary keys  
- Foreign keys  
- Relationships  

Main tables:

- `Hotel`
- `Room`
- `Staff`
- `Guests`
- `Payment`
- `Reservation`
- `Serves`
- `Make`
- `G_email`
- `G_Pt`
- `H_Pt`

> The schema diagram (page 3) illustrates how tables are connected through keys and constraints :contentReference[oaicite:2]{index=2}.

---

##  SQL Implementation

###  Table Creation

Example:

```sql
CREATE TABLE Hotel (
    H_num INT PRIMARY KEY,
    Name VARCHAR(100) NOT NULL,
    Location VARCHAR(100) NOT NULL,
    Star_rating INT NOT NULL DEFAULT 1
);
````

The project includes full SQL scripts for:

* Table creation
* Relationships (foreign keys)
* Constraints

---

###  Data Insertion

Sample data is inserted into all tables:

```sql
INSERT INTO Hotel VALUES 
(1, 'Four Seasons', 'Alexandria', 5),
(2, 'Hilton', 'King', 4);
```

> Data insertion examples are shown across pages 7–15 .

---

###  Queries & Analysis

The project includes SQL queries such as:

* Retrieve guests with specific conditions
* Calculate average staff salary
* Count total number of guests

Example:

```sql
SELECT AVG(Salary)
FROM Staff;
```

> Query results and examples are shown in the bonus section (page 18) .

---

##  System Functionality

The database supports:

* Managing hotel and room data
* Tracking reservations and availability
* Storing guest information
* Managing staff roles and salaries
* Handling payments

---

##  Technologies Used

* **SQL (MySQL / relational database concepts)**
* Database design principles (ERD, normalization)

---

##  Project Structure

```
project/
│── report.pdf        # Full documentation
│── README.md
```

---

##  Project Report

👉 Full documentation available here:
[View Report](DBproj.pdf)

---

##  What I Learned

* Designing relational databases
* Creating ER diagrams and schemas
* Writing SQL queries (DDL & DML)
* Using primary and foreign keys
* Applying normalization concepts
* Structuring real-world systems

---

##  Limitations

* No GUI or application layer
* Static dataset (no dynamic updates)
* No stored procedures or triggers

---

##  Future Improvements

* Integrate with backend (Node.js / Python)
* Add user interface (web app)
* Implement advanced queries
* Add indexing for performance
* Use stored procedures and triggers

---

##  Team Members

* Laila Tarek
* Hana Tariq
* Abdallah Nizar
* Hazem Mohab

---

##  Disclaimer

This project is for **educational purposes only**.

```

