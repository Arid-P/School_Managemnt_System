# 🏫 School Management System 3.0 (`with_ai_gui` branch)

A modern School Management System web interface built using **Streamlit**, **Pandas**, and **SQLAlchemy**, managed with [`uv`](https://docs.astral.sh/uv/).

---

## 🚀 Features

- **Streamlit Web Interface**: Clean, responsive, and intuitive web dashboard for student and teacher management.
- **Search & Filtering**: Real-time search of students and teachers by name.
- **Full CRUD Operations**:
  - **Students**: Add, update (grade/phone/name), and delete student records.
  - **Teachers**: Add, update (subject/phone/name), and delete teacher records.
- **Data Display**: Formatted tables and live dataframes powered by Pandas.
- **Persistent Storage**: SQLite database backend powered by SQLAlchemy ORM.
- **CLI Mode**: Interactive terminal menu interface (`main.py`) for command-line operation.

---

## 🌿 Branches & Variants

- **`with_ai_gui`** *(current)*: Contains the **Streamlit** web application (`app.py`).
- **`main`**: The base project branch featuring the **PySide6 (Qt desktop GUI)** interface.

---

## 🛠️ Requirements & Installation

This project is managed using [`uv`](https://docs.astral.sh/uv/).

### Prerequisites

- Python 3.12+ (or 3.14+)
- [`uv`](https://docs.astral.sh/uv/getting-started/installation/)

### Setup

Clone the repository and switch to the `with_ai_gui` branch:

```bash
git clone https://github.com/Arid-P/School_Managemnt_System.git
cd School_Managemnt_System
git checkout with_ai_gui
uv sync
```

---

## 💻 Running the Application

### 1. Streamlit Web Interface

Launch the interactive web application:

```bash
uv run streamlit run app.py
```

The app will automatically open in your browser (typically at `http://localhost:8501`).

### 2. Command Line Interface (CLI)

Run the CLI menu:

```bash
uv run python main.py
```

---

## 📂 Project Structure

```
.
├── .gitignore
├── pyproject.toml              # Project metadata & dependencies (Streamlit, Pandas, SQLAlchemy)
├── uv.lock                     # Locked dependencies
├── app.py                      # Streamlit web application entrypoint
├── main.py                     # CLI entrypoint
├── school.db                   # SQLite database (auto-generated)
├── Logging/                    # Application logs
└── school_models/              # SQLAlchemy database models & logic
    ├── tables.py               # Database schemas (Students, Teachers)
    ├── student.py              # Student CRUD operations
    ├── teacher.py              # Teacher CRUD operations
    └── validity_checking.py   # Phone number and name validation rules
```

---

## 📄 License

This project is open source and available under the MIT License.
