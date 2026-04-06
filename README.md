# 🎓 PyQt6 Student Management System

A lightweight, desktop-based graphical user interface (GUI) application designed to manage student records. Built entirely in Python, this system leverages PyQt6 for a responsive frontend and integrates a local SQLite database for persistent, serverless data storage.

## 🧠 Engineering Architecture
This application utilizes a tightly coupled Model-View architecture:
* **Frontend (View):** Constructed with `PyQt6.QtWidgets`. It utilizes a `QMainWindow` for the primary dashboard and dynamic `QDialog` instances for data entry and modification.
* **Backend (Model):** Powered by Python's built-in `sqlite3` library. SQL queries (`SELECT`, `INSERT`, `UPDATE`, `DELETE`) are executed directly through a custom `DatabaseConnection` class, mapping GUI inputs to permanent storage.

## ⚙️ Core Features
* **CRUD Operations:** Full lifecycle management of student records (Create, Read, Update, Delete) integrated directly into the GUI.
* **Dynamic Data Table:** Implements `QTableWidget` to render the database in real-time. Selecting a row dynamically triggers contextual actions (Edit/Delete).
* **Targeted Search:** Includes a dedicated locator tool using `Qt.MatchFlag.MatchFixedString` to query the database and visually highlight exact matches within the main data table.
* **Stateless Initialization:** Automatically generates and connects to `database.db` upon launch, requiring zero manual database configuration.

## 🛠️ Tech Stack
* **Language:** Python 3.10+
* **GUI Framework:** PyQt6
* **Database:** SQLite3
* **System Libraries:** `sys`

## 🚀 Installation & Execution

Follow the exact bash commands below to isolate the environment and launch the application locally.

**1. Clone the repository**
```bash
git clone https://github.com/Nayanxyz/student-management-system.git
cd student-management-system
```
