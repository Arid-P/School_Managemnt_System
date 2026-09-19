# 🏫 School Management System

A Python-based School Management System featuring both a CLI interface and a desktop GUI powered by PySide6 (Qt) and SQLAlchemy, managed with [`uv`](https://docs.astral.sh/uv/).

---

## 🚀 Features

- **Student Management**: Add, view, search, update, and remove students (tracking ID, Name, Phone Number, Grade).
- **Teacher Management**: Add, view, search, update, and remove teachers (tracking ID, Name, Phone Number, Subject).
- **Validation**: Built-in phone number and name validations.
- **Persistent Storage**: SQLite database backend powered by SQLAlchemy ORM.
- **Desktop GUI**: Built with PySide6 featuring a dark theme, intuitive forms, and responsive tables.
- **CLI Mode**: Interactive terminal menu interface for quick administration.
- **Logging**: Comprehensive application logging for auditing and debugging.

---

## 🌿 Branches & Variants

- **`main`** *(current)*: Contains the core application with the **PySide6 (Desktop Qt)** GUI and terminal interface.
- **`with_ai_gui`**: An alternative branch featuring a **Streamlit** web-based dashboard interface.

---

## 🛠️ Requirements & Installation

This project is managed using [`uv`](https://docs.astral.sh/uv/).

### Prerequisites

- Python 3.12+ (or 3.14+)
- [`uv`](https://docs.astral.sh/uv/getting-started/installation/)

### Setup

Clone the repository and install dependencies:

```bash
git clone https://github.com/Arid-P/School_Managemnt_System.git
cd School_Managemnt_System
uv sync
```

---

## 💻 Running the Application

### 1. PySide6 Desktop GUI

To launch the graphical user interface:

```bash
uv run python gui/app.py
```

### 2. Command Line Interface (CLI)

To launch the terminal-based menu:

```bash
uv run python main.py
```

---

## 📂 Project Structure

```
.
├── .gitignore
├── pyproject.toml              # Project metadata & dependencies
├── uv.lock                     # Locked dependencies
├── main.py                     # CLI entrypoint
├── school.db                   # SQLite database (auto-generated)
├── Logging/                    # Application logs
├── school_models/              # Core business logic & ORM tables
│   ├── tables.py               # SQLAlchemy models (Students, Teachers)
│   ├── student.py              # Student CRUD operations
│   ├── teacher.py              # Teacher CRUD operations
│   └── validity_checking.py   # Phone & name validation rules
└── gui/                        # PySide6 GUI package
    ├── app.py                  # Main GUI window
    ├── theme.py                # UI Dark theme stylesheet
    ├── logger.py               # GUI logging configuration
    ├── adapters/               # Backend data adapters
    ├── controllers/            # MVC controllers
    ├── views/                  # Main, student & teacher views
    └── widgets/                # Form & table reusable widgets
```

---

## 📄 License

This project is open source and available under the MIT License.
