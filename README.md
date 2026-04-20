## Inventory Management System

A robust, role-based Inventory Management System built with a **Python (Flask)** backend and an **HTML/JavaScript** frontend. This system streamlines business operations by providing specific dashboards for administrators, store managers, sales teams, and cashiers.

---

## 🚀 Getting Started

### Prerequisites
* **Python 3.x** installed from [python.org](https://www.python.org/)
* **Git** installed on your local machine

### Installation & Setup

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/sami9644/Inventory-Management-System-in-python-and-html.git
    cd Inventory-Management-System-in-python-and-html
    ```

2.  **Install Dependencies**
    Install the required Python packages using pip:
    ```bash
    pip install flask flask-cors
    ```

3.  **Database Initialization**
    Before running the application, you must initialize the database:
    * Open `db.py`.
    * Locate and **uncomment** the `create_db()` function call.
    * Run the script:
        ```bash
        python db.py
        ```

---

## 🛠️ Running the Application

### 1. Admin Dashboard
Launch the admin panel to manage staff and organizational settings:
```bash
python app.py
```
* **Capabilities:** Add, view, and remove employee records.

### 2. Employee Services & API
Launch the backend API to enable employee functionalities:
```bash
python apirequests.py
```

### 3. Employee Access
* Navigate to the `users/employee` folder.
* create a server writing this command
  ```bash
  python -m http.server 8000
  ```
  then write [127.0.0.1:8000](http://127.0.0.1:8000)
* Registered employees can set their passwords and log in to their specific dashboards.

---

## 👥 User Roles & Permissions

The system utilizes a granular role-based access control (RBAC) model:

| Role | Responsibility |
| :--- | :--- |
| **Admin** | Employee lifecycle management (Hire/Fire). |
| **Store Manager** | Full CRUD operations on inventory items. |
| **Sales** | Creation and initiation of pending orders. |
| **Picker** | Processing and finalizing pending orders. |
| **Cashier** | Generating receipts for completed orders. |

---

## 💻 Tech Stack
* **Backend:** Python, Flask
* **Frontend:** HTML5, CSS3, JavaScript
* **Middleware:** Flask-CORS for cross-origin resource sharing
* **Database:** SQLite (managed via `db.py`)
