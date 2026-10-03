# 🐘 PostgreSQL — Users, Logins, Databases & Roles

> 🎓 **Hands-On PostgreSQL Training**
>
> Learn how to create users, manage login roles, configure privileges, and prepare your PostgreSQL environment for database and table practice.

---

## 📚 What You'll Learn

- 👤 PostgreSQL Users & Roles
- 🔐 Login & Authentication
- 🛡️ User Privileges
- 👑 Superuser vs Normal User
- 🗄️ Database Management
- 📂 Schemas
- 📋 Tables
- 👥 Role Membership
- ⚙️ Role Configuration
- 🖥️ Working with pgAdmin

---

## 🗄️ 1. Explore the PostgreSQL Server

After connecting to your PostgreSQL server through **pgAdmin**, expand the server to explore its different components.

You'll find sections such as:

- 🗄️ **Databases**
- 👥 **Login/Group Roles**
- ⚙️ **Server Configuration**
- 📊 **Replication**
- 🔧 Other administration options

PostgreSQL organizes its data and security objects in a structured hierarchy, making database management easier.

---

## 🗃️ 2. Explore the Default Database

When PostgreSQL is installed, a default database named **postgres** is generally available.

You can find it under the **Databases** section.

Inside the database, you'll find:

**Schemas → Tables**

The **public schema** is commonly available by default.

At the beginning of our training environment, there may not be any user-created tables.

We'll create our own training databases and tables as we progress. 🚀

---

## 👤 3. Understand the Default PostgreSQL User

During installation, PostgreSQL normally creates a default administrative user named **postgres**.

This account has **superuser privileges**.

A superuser has extensive control over the PostgreSQL server and can perform administrative operations such as:

- Creating databases
- Removing databases
- Creating users and roles
- Managing permissions
- Performing administrative tasks

### ⚠️ Important

For everyday application access, it is generally better to use a dedicated account with only the permissions it requires.

This follows the **principle of least privilege**. 🔐

---

## 🆕 4. Create a New User

Now let's create our first training user.

### 👤 User Name

**Adam**

We'll use this account throughout our PostgreSQL practice.

### 📍 In pgAdmin

Go to:

**Login/Group Roles → Right Click → Create → Login/Group Role**

A configuration window will appear where we can define the user's settings.

---

## 📝 5. Configure the User

Enter the role name:

### 👤 Adam

The role name identifies the account within PostgreSQL.

After entering the name, we can configure authentication and privileges.

---

## 🔐 6. Set the Password

Navigate to the **Definition** section.

Here you can specify a password for the user.

### 🔒 Password Best Practices

Always use a strong and unique password.

Avoid simple passwords such as:

- ❌ password
- ❌ 123456
- ❌ admin
- ❌ postgres

For real-world systems, credentials should be securely stored and managed.

---

## 🛡️ 7. Configure User Privileges

The **Privileges** section controls what the role is allowed to do.

For our training user, configure the account as follows:

| Permission | Setting |
|---|---|
| 🔑 Can Login | ✅ Yes |
| 👑 Superuser | ❌ No |
| 👥 Create Roles | ❌ No |
| 🗄️ Create Databases | ✅ Yes |
| 🔄 Replication | ❌ No |

This gives Adam enough access for our training exercises without providing unrestricted administrative access.

---

## 🔑 Understanding the Privileges

### 🔑 Can Login

Allows the user to connect to PostgreSQL.

Without login permission, the role cannot be used as a normal login account.

---

### 👑 Superuser

A superuser has extremely broad administrative privileges.

For our training account:

**Superuser → No**

This allows us to practice using a normal PostgreSQL role rather than an unrestricted administrator account.

---

### 👥 Create Roles

Controls whether the user can create and manage other PostgreSQL roles, subject to PostgreSQL's privilege model.

For Adam:

**Create Roles → No**

---

### 🗄️ Create Databases

Allows Adam to create databases.

For our training environment:

**Create Databases → Yes**

We'll use this capability in upcoming exercises.

---

### 🔄 Replication

Replication-related privileges are used for PostgreSQL replication and related administrative operations.

For our current training:

**Replication → No**

We'll explore replication separately when we reach advanced PostgreSQL administration.

---

## 👥 8. Role Membership

The **Membership** section allows a role to become a member of another role.

This is useful when working with groups and shared permissions.

Organizations can create different group roles for:

- 👨‍💻 Developers
- 🧑‍💼 Analysts
- 🛠️ Database Administrators
- 👀 Read-Only Users

Users can then receive permissions through their group memberships.

For now, we'll leave Adam's membership settings unchanged.

---

## ⚙️ 9. Parameters

The **Parameters** section allows PostgreSQL configuration parameters to be customized for a particular role.

These settings are useful for advanced database administration and workload-specific configurations.

For our current training, we'll keep the default settings.

---

## 💻 10. The SQL Section

One of the most useful features in pgAdmin is the **SQL** section.

Whenever you configure something through the graphical interface, pgAdmin can show the SQL operation associated with your choices.

This is an excellent way to learn PostgreSQL.

### 💡 Learning Tip

Don't just click buttons in pgAdmin.

Whenever possible:

**Configure it in pgAdmin → Look at the generated SQL → Understand what it does**

This will help you gradually move from GUI-based administration to writing PostgreSQL commands yourself.

---

## 💾 11. Save the New User

Once all the settings have been configured:

### 👉 Click **Save**

The new login role will be created.

You should now be able to find **Adam** under:

**Login/Group Roles**

🎉 **Your first PostgreSQL training user is ready!**

---

## 🔍 12. Verify the User

Right-click on **Adam** and open **Properties**.

Review the settings to confirm that the account has the intended permissions.

Verify that:

- ✅ Login is enabled
- ❌ Superuser is disabled
- ❌ Role creation is disabled
- ✅ Database creation is enabled
- ❌ Replication is disabled

This is a good habit whenever you create or modify database accounts.

---

## 🧠 PostgreSQL Concepts to Remember

| Concept | Meaning |
|---|---|
| 👤 **Role** | PostgreSQL identity used for users and groups |
| 🔑 **Login** | Allows a role to connect to PostgreSQL |
| 👑 **Superuser** | Provides extensive administrative privileges |
| 🗄️ **Create Database** | Allows a role to create databases |
| 👥 **Create Role** | Allows role-management capabilities |
| 📂 **Schema** | Logical namespace for database objects |
| 📋 **Table** | Stores structured data |
| 🔐 **Privilege** | Permission to perform an operation |

---

## ⭐ Key Takeaways

### 🐘 PostgreSQL uses **roles** to manage users and groups.

The default **postgres** account is typically a superuser, while our **Adam** account is a more restricted training account.

### 🔐 Remember

**Superuser ≠ Normal User**

A superuser has broad administrative control, while a normal role can be configured with only the permissions it needs.

### 💡 Best Practice

> **Give users only the permissions they actually need.**

This makes database environments easier to manage and helps reduce unnecessary security exposure.

---

## 🚀 What's Next?

Our PostgreSQL environment is now ready for the next stage.

We'll move from:

**👤 Users & Roles**

to:

**🗄️ Databases → 📂 Schemas → 📋 Tables → 📊 Data → 🔎 Queries**

That's where we'll start doing real PostgreSQL hands-on practice. 🐘💻

---

## 🎯 Happy Learning!

> **Learn the GUI. Understand the SQL. Master PostgreSQL.** 🚀