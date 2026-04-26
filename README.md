# Library-Management-System-Python-Tkinter-SQLite


A desktop **Library Management System** built with **Python**, **Tkinter**, and **SQLite**. Developed as the SSX361 Scripting & Syntax assessment at Belgium Campus iTVersity.

The application allows library staff to manage books and member records through a clean graphical interface, with full CRUD operations backed by a local SQLite database.

---

## Features

### Book Management
- Add new books with title, author, ISBN, genre, and availability status
- View all books in a sortable table
- Update existing book information
- Delete books from the system
- Search books by title, author, or ISBN

### Member Management
- Register new members with membership ID, name, surname, contact, and membership type
- View all members sorted alphabetically
- Update member information
- Delete members from the system
- Search members by ID, name, or surname

---

## Screenshots

> Run the application to see the GUI in action.

---

## Tech Stack

| Category | Technology |
|----------|-----------|
| Language | Python 3 |
| GUI | Tkinter / ttk |
| Database | SQLite3 |
| IDE | PyCharm |

---

## Project Structure

```
library-management-system/
├── main.py          # Main application entry point — GUI for books and members
├── books_db.py      # Database operations for books (CRUD + search)
├── members_db.py    # Database operations for members (CRUD + search)
├── library.db       # SQLite database (auto-created on first run)
└── README.md
```

---

## How It Works

The application follows a simple layered structure:

- **GUI Layer** (`main.py`) — Tkinter windows for Book Manager and Member Manager. Handles all user interaction, form input, and table display.
- **Data Layer** (`books_db.py`, `members_db.py`) — All database operations using Python's built-in `sqlite3` module. Each file handles its own table with full CRUD and search functionality.
- **Database** (`library.db`) — SQLite database with two tables: `books` and `members`. Auto-created on first run.

---

## Database Schema

### Books Table
| Column | Type | Description |
|--------|------|-------------|
| id | INTEGER | Primary key, auto-incremented |
| title | TEXT | Book title (required) |
| author | TEXT | Author name (required) |
| isbn | TEXT | Unique ISBN (required) |
| genre | TEXT | Book genre (optional) |
| availability | TEXT | Available / Not Available |

### Members Table
| Column | Type | Description |
|--------|------|-------------|
| membership_id | TEXT | Primary key |
| name | TEXT | First name (required) |
| surname | TEXT | Surname (required) |
| contact | TEXT | Contact details (optional) |
| membership_type | TEXT | Student / Regular / Premium |

---

## Getting Started

### Prerequisites
- Python 3.x installed
- No external libraries required — uses only Python standard library

### Run the Application

```bash
# Clone the repository
git clone https://github.com/GivenMoreke/library-management-system.git

# Navigate into the project folder
cd library-management-system

# Run the application
python main.py
```

The SQLite database will be created automatically on first run.

---

## Key Concepts Demonstrated

- Python scripting and object-oriented programming with classes
- Building desktop GUIs with Tkinter and ttk widgets
- SQLite database operations using Python's `sqlite3` module
- Full CRUD implementation (Create, Read, Update, Delete)
- Search functionality using SQL LIKE queries
- Input validation and error handling
- Separation of concerns — GUI and database logic in separate files
- Event-driven programming (button clicks, table row selection)

---

## Author
Reitumetse Given Moreke
**Reitumetse Given Moreke**
Diploma in Information Technology — Belgium Campus iTVersity
[LinkedIn](#) | [GitHub](https://github.com/GivenMoreke)
