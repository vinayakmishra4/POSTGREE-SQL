# 🐘 PostgreSQL Sample Database Setup

Welcome! 👋

In this lesson, we’ll populate our PostgreSQL database with **sample data** that will be used throughout the upcoming video series.

We’ll create three tables:

- 👤 **Customers**
- 📦 **Products**
- 🛒 **Purchases**

> 💡 **Goal:** Set up the sample database so we can focus on learning SQL concepts in the upcoming lessons.

---

## 📥 Step 1: Download the SQL Files

The sample SQL files are provided in the **Downloads** section of the course introduction.

Download the following files to your local computer:

```text
customers.sql
products.sql
purchases.sql
```

Keep all three files in an easily accessible folder.

---

# 🛠️ Step 2: Open pgAdmin

Launch **pgAdmin** and open the **Query Tool**.

Before opening a file, make sure the query editor is empty.

### 📌 Open the Customers File

1. Click **Open File** 📂
2. Navigate to the folder where you downloaded the SQL files.
3. Select:

```text
customers.sql
```

4. Click **Select**.

The SQL commands will now appear in the Query Tool.

The script will:

- Create the `customers` table
- Add sample customer records
- Define the required **Primary Key**

### ▶️ Run the Script

Click the **Run** ▶️ button to execute the SQL script.

After the script finishes:

1. Go to the **Tables** section in pgAdmin.
2. Right-click on **Tables**.
3. Select **Refresh** 🔄.

You should now see:

```text
customers
```

🎉 **Customers table created successfully!**

---

# 📦 Step 3: Create the Products Table

Now let's create our second table.

First, clear the Query Tool:

```text
Ctrl + A → Delete
```

> 🍎 On Mac, use **Command + A**.

Then:

1. Click **Open File** 📂
2. Select:

```text
products.sql
```

3. Click **Select**.
4. Click **Run** ▶️.

This script will create the `products` table and populate it with sample data.

It also defines the required **Primary Key**.

Refresh the **Tables** section again.

You should now have:

```text
customers
products
```

🎉 **Products table created successfully!**

---

# 🛒 Step 4: Create the Purchases Table

Finally, we'll create the `purchases` table.

Clear the Query Tool again:

```text
Ctrl + A → Delete
```

Then:

1. Click **Open File** 📂
2. Select:

```text
purchases.sql
```

3. Click **Select**.
4. Click **Run** ▶️.
5. Refresh the **Tables** section.

The script will create the `purchases` table along with:

- 🗝️ Primary Key
- 🔗 Foreign Keys
- 📊 Sample purchase records

---

# 🎯 Final Database Structure

After completing all three steps, your database should contain:

```text
📁 Tables
│
├── 👤 customers
├── 📦 products
└── 🛒 purchases
```

### 🔗 Table Relationships

The `purchases` table uses **foreign keys** to establish relationships with other tables.

A simplified view:

```text
        👤 CUSTOMERS
             │
             │
             ▼
        🛒 PURCHASES
             ▲
             │
             │
        📦 PRODUCTS
```

These relationships will become important when we start working with **JOINs, relationships, and database queries**.

---

# 🧠 What We've Accomplished

By the end of this setup, you should have:

| Table | Purpose |
|---|---|
| 👤 `customers` | Stores customer information |
| 📦 `products` | Stores product information |
| 🛒 `purchases` | Stores purchase/transaction information |

---

## 🚀 What's Next?

Now that our sample database is ready, we're all set to start working with SQL!

In the upcoming lessons, we'll learn how to:

- 🏗️ Create tables
- ➕ Insert records
- 🔍 Retrieve data
- ✏️ Update records
- 🗑️ Delete records
- 🔑 Work with Primary Keys
- 🔗 Work with Foreign Keys
- 🔀 Join multiple tables
- 📊 Write useful SQL queries

> ⭐ **Remember:** For now, don't worry about understanding every SQL command inside these files. The purpose of this lesson is simply to **set up the sample database**. We'll learn how everything works step by step in the upcoming videos.

---

### ✅ Setup Checklist

- [ ] Download `customers.sql`
- [ ] Create the `customers` table
- [ ] Download/use `products.sql`
- [ ] Create the `products` table
- [ ] Download/use `purchases.sql`
- [ ] Create the `purchases` table
- [ ] Refresh pgAdmin
- [ ] Verify all three tables are visible

🎉 **Your PostgreSQL sample database is now ready!**x