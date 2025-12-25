

---

### ✅ **Django Setupy Steps & Notes**

#### 1. **Virtual Environment (Always First!)**
-  **Activate it first** before installing anything:
  ```bash
  source venv/bin/activate      # Linux/macOS
  venv\Scripts\activate         # Windows
  ```
- Keeps dependencies isolated — best practice.

---

#### 2. **Installing Django**

  ```bash
  pip install Django
  ```

---

#### 3. **Creating a Django Project**
- **Basic command**:
  ```bash
  django-admin startproject projectname
  ```
  → Creates nested folder: `projectname/projectname/`

- ✅ **Recommended (flat structure)** — use `.` to avoid duplication:
  ```bash
  django-admin startproject company .
  ```
  → Creates files directly in current folder (manage.py at root + `company/` config folder).

---