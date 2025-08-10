## **Library Management System (Python + Jupyter Notebook)**

**Repository URL:** `https://github.com/arnab236/Library-Management-System-Analysis`

### Overview

This project offers a lightweight, interactive **Library Management System** developed using **Python** in a **Jupyter Notebook** environment. It empowers you to manage library operations — like searching books, tracking borrow/return events, and analyzing usage — entirely via CSV files.

---

### Features

1. **CSV-Based Data Management**

   * Loads data from CSV files for `books`, `authors`, `members`, and `borrowingrecords` from a configurable directory (`./CSVFiles` by default).
   * Includes fallback sample data when CSVs are missing, ensuring the notebook runs regardless.

2. **Interactive Search Interface**

   * Live search widget allowing filtering by **title**, **author**, **genre**, or **book ID**.
   * Efficient author-book lookup using merged data for fast response.

3. **Borrow / Return Simulation**

   * Borrow books with availability checks.
   * Return books and automatically update member stats and CSV files.
   * All changes are written back to the source CSVs for persistence.

4. **Analytical Reports & Visualizations**

   * **Top borrowed books**: See which books are most frequently checked out.
   * **Most active members**: Find members with the most borrow activity.
   * **Availability overview**: Snapshot showing which books are currently borrowed versus available.
   * **Overdue items**: List borrow records past their return date.
   * Visualized charts (bar graphs) for quick insights.

5. **User-Friendly Interface**

   * Widgets driven interface makes it easy to interactively manage your library.
   * Single-click “Save CSVs” to persist states.

---

### Project Structure

```
Library-Management-System-Python-/
├── CSVFiles/                         ← Where your CSVs go
│   ├── library_books.csv
│   ├── library_authors.csv
│   ├── library_members.csv
│   └── library_borrowingrecords.csv
├── library_management_notebook.ipynb ← Main interactive notebook
├── requirements.txt                  ← Python dependencies
└── README.md                         ← This documentation
```

---

### Getting Started

1. **Clone the repository:**

   ```bash
   git clone https://github.com/arnab236/Library-Management-System-Analysis.git
   cd Library-Management-System-Python-
   ```

2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Add your CSV files** to the `CSVFiles/` directory. If they’re missing, the notebook will use sample data.

4. **Open the notebook:**

   ```bash
   jupyter notebook library_management_notebook.ipynb
   ```

5. **Run cells in order** and interact with the notebook:

   * Use the search box to explore books.
   * Simulate borrows and returns.
   * View analysis and charts.
   * Save changes when done.

---

### Future Enhancements (Ideas)

* Support **fine calculation** or overdue notifications.
* Export reports (e.g., Excel, PDF).
* Transition to a web app (Flask or Streamlit) using this notebook logic as backend.

---

### Dependencies

Listed in `requirements.txt`:

* pandas
* matplotlib
* ipywidgets

(This notebook runs out-of-the-box with the above installed.)

---

