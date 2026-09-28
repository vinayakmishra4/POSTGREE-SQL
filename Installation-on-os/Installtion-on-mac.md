# 🐘 Installing PostgreSQL on Mac

A simple guide to installing **PostgreSQL** on macOS.

---

## 📌 Prerequisites

- macOS
- Internet connection
- Administrator access to your Mac

---

## 🚀 1. Download PostgreSQL

1. Visit the official PostgreSQL website.
2. Click **Download**.
3. Select **macOS**.
4. Choose **Download the installer**.
5. Select the PostgreSQL version you want to install.

> 💡 **Note:** The original tutorial uses PostgreSQL **12.4**. For a fresh installation, use a currently supported PostgreSQL release when possible.

---

## 💿 2. Launch the Installer

After downloading the installer:

1. Locate the downloaded file.
2. Double-click it.
3. If macOS asks for permission, click **Open**.
4. Follow the installation wizard.

---

## 📦 3. Select Components

The installer provides several components:

| Component | Description |
|---|---|
| 🐘 PostgreSQL Server | Database server |
| 🖥️ pgAdmin 4 | GUI for managing databases |
| 🧰 Stack Builder | Additional PostgreSQL tools |
| ⌨️ Command Line Tools | PostgreSQL terminal utilities |

Keep the default components selected unless you have a specific requirement.

Click **Next**.

---

## 📁 4. Choose Installation Directory

Select the directory where PostgreSQL will be installed.

For most users, the **default location** is recommended.

Click **Next**.

---

## 🔐 5. Create a Password

Create a password for the PostgreSQL **superuser**.

For local development, choose a secure password that you can remember.

> ⚠️ Never use weak or reused passwords on production systems.

Click **Next**.

---

## 🔌 6. Configure the Port

PostgreSQL uses a port to accept database connections.

The default port is:

```text
5432
```

Unless you need a different port, keep the default value.

Click **Next**.

---

## 🌎 7. Select the Locale

Choose the locale for your PostgreSQL installation.

For most users, the default option is sufficient.

Click **Next**.

---

## ✅ 8. Review & Install

Review the installation settings:

- Installation directory
- PostgreSQL components
- Superuser password
- Port
- Locale

If everything looks correct, click **Next** to begin the installation.

Wait for the installation to complete.

---

## 🎉 9. Installation Complete

Once installation finishes, PostgreSQL is ready to use.

You can manage your databases using:

- 🖥️ **pgAdmin 4**
- ⌨️ **Command Line Tools**
- 🐘 PostgreSQL-compatible applications

---

## 🧪 10. Verify Installation

Open **Terminal** and run:

```bash
psql --version
```

If PostgreSQL is correctly installed and available in your PATH, the command will display the installed version.

---

## ⚙️ Default Configuration

| Setting | Default |
|---|---|
| Database System | PostgreSQL |
| Port | `5432` |
| GUI | pgAdmin 4 |
| Platform | macOS |

---

## 🔄 Installation Flow

```text
Download PostgreSQL
        ↓
Open Installer
        ↓
Select Components
        ↓
Choose Installation Directory
        ↓
Set Superuser Password
        ↓
Configure Port
        ↓
Select Locale
        ↓
Review Settings
        ↓
Install PostgreSQL
        ↓
Verify Installation
```

---

## 🎯 You're Ready!

PostgreSQL is now installed on your Mac.

You can use **pgAdmin 4** for a graphical interface or **Terminal** to work with PostgreSQL from the command line.

> 🐘 **Happy coding!**