# 🎬 PostgreSQL — Creating & Modifying Tables

<p align="center">
  <img src="https://img.shields.io/badge/Database-PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Language-SQL-orange?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL">
  <img src="https://img.shields.io/badge/Project-Learning-success?style=for-the-badge" alt="Learning Project">
</p>

<p align="center">
  <strong>📚 Exploring PostgreSQL through a real-world Movies Database</strong>
  <br>
  Learn how to create, modify, and manage relational database tables.
</p>

---

## 📌 About the Project

This project demonstrates fundamental **PostgreSQL table creation and modification** concepts using a Movies database.

The database organizes information into four tables: Movies, Actors, Directors, and Movie Revenue. Through this project, you can explore relational database design, table structures, data types, keys, constraints, and relationships.

The goal is to build a practical understanding of how database tables are created and modified as data requirements evolve.

## 📑 Table of Contents

- [🗄️ Database Structure](#️-database-structure)
- [🏗️ Creating Tables](#️-creating-tables)
- [🛠️ Modifying Tables](#️-modifying-tables)
- [🔗 Table Relationships](#-table-relationships)
- [✨ Key Concepts](#-key-concepts)
- [✅ Best Practices](#-best-practices)
- [🎯 Learning Objectives](#-learning-objectives)
- [📂 SQL Script](#-sql-script)
- [🏁 Conclusion](#-conclusion)

---

## 🗄️ Database Structure

The Movies database consists of four main tables, each designed to organize a specific category of information.

| 🎬 Table | 📝 Description |
|:---|:---|
| 🎞️ **Movies** | Stores information about movies and their details. |
| 🎭 **Actors** | Organizes information about actors associated with movies. |
| 🎬 **Directors** | Stores information about movie directors. |
| 💰 **Movie Revenue** | Organizes financial information related to movie revenue. |

> 💡 **Database design principle:** Separating information into related tables helps organize data and can reduce unnecessary duplication.

*For the exact columns, data types, constraints, and relationships, refer to the SQL script linked below.*

---

## 🏗️ Creating Tables

Table creation is one of the fundamental operations in PostgreSQL. It defines how information is organized and stored within a database.

When designing a table, several elements are important:

- **Table Names:** Identify the category of information being stored.
- **Columns:** Define the individual attributes of each record.
- **Data Types:** Specify the kind of values a column can contain.
- **Primary Keys:** Uniquely identify records.
- **Constraints:** Help maintain data accuracy and consistency.

A well-designed table structure provides a strong foundation for managing relational data.

## 🛠️ Modifying Tables

Database requirements can change over time. PostgreSQL supports modifications to existing table structures so that the database can adapt without necessarily recreating entire tables.

Common table modification operations include:

| Operation | Purpose |
|:---|:---|
| ➕ **Add Columns** | Introduce new attributes into an existing table. |
| 🔧 **Modify Column Definitions** | Change supported column properties or data types. |
| ✏️ **Rename Columns** | Improve column names for clarity. |
| 🏷️ **Rename Tables** | Update table names to better reflect their purpose. |
| ➖ **Drop Columns** | Remove attributes that are no longer required. |
| 🛡️ **Manage Constraints** | Add or remove rules governing the data. |

> ⚠️ **Important:** Some table modifications can affect existing data and dependent database objects. Review potential impacts before making destructive changes.

---

## 🔗 Table Relationships

Relational databases allow information stored in different tables to be connected.

In a Movies database, relationships may connect movies with actors, directors, and revenue records, depending on the implemented schema.

Two important concepts are:

**🔑 Primary Key**
- Uniquely identifies a record within a table.
- Helps prevent duplicate record identifiers.

**🔗 Foreign Key**
- Establishes a reference to a key in another table.
- Helps maintain referential integrity when a relationship is enforced.

Well-planned relationships make a database easier to maintain and query.

---

## ✨ Key Concepts

This project covers several essential database concepts:

| Concept | What It Means |
|:---|:---|
| 🗄️ **Database** | An organized collection of related information. |
| 📋 **Table** | A structure that stores data in rows and columns. |
| 🧱 **Schema** | The structure and organization of database objects. |
| 🔢 **Data Types** | Define the types of values stored in columns. |
| 🔑 **Primary Key** | Uniquely identifies a record. |
| 🔗 **Foreign Key** | Connects related records across tables. |
| 🛡️ **Constraints** | Enforce rules on the data. |
| 🔧 **Table Modification** | Changes an existing table's structure. |

---

## ✅ Best Practices

When working with PostgreSQL, consider the following recommendations:

- 📌 Use meaningful and consistent table and column names.
- 📌 Select appropriate data types for each column.
- 📌 Define primary keys where unique record identification is required.
- 📌 Use foreign keys when relationships should be enforced.
- 📌 Apply suitable constraints to maintain data integrity.
- 📌 Check dependencies before removing columns or constraints.
- 📌 Verify table structures after making changes.
- 📌 Back up important data before potentially destructive operations.
- 📌 Use transactions when appropriate to manage related database changes safely.

---

## 🎯 Learning Objectives

By completing this project, you can develop a practical understanding of:

- Creating tables in PostgreSQL.
- Modifying existing table structures.
- Working with columns and data types.
- Understanding primary keys and foreign keys.
- Applying constraints to maintain data integrity.
- Organizing information across multiple relational tables.
- Following good database design practices.

---

## 📂 SQL Script

Want to explore the actual implementation?

<p align="center">
  <a href="https://github.com/vinayakmishra4/POSTGREE-SQL/blob/main/Create-and-Modifiying/movie_database.sql">
    <img src="https://img.shields.io/badge/View_SQL_Script-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="View SQL Script on GitHub">
  </a>
</p>

**📄 File:** `movie_database.sql`

The script contains the SQL implementation for the Movies database.

**👉 [Click here to view the complete SQL script](https://github.com/vinayakmishra4/POSTGREE-SQL/blob/main/Create-and-Modifiying/movie_database.sql)**

---

## 🏁 Conclusion

This project provides a practical introduction to **creating and modifying tables in PostgreSQL** through a Movies database.

By organizing information into Movies, Actors, Directors, and Movie Revenue tables, the project demonstrates foundational concepts in relational database design and table management.

These skills provide a foundation for working with more complex databases and developing reliable data-driven applications.

---

<p align="center">
  <strong>🚀 Keep Learning. Keep Building. Keep Querying.</strong>
  <br><br>
  Made with ❤️ while learning PostgreSQL
</p>