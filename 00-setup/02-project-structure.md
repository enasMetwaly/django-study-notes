

#### 4. **Structure Files  & Their Purpose**

| File | Purpose | Notes |
|------|---------|-------|
| `__init__.py` | Marks folder as a Python **module** | Usually empty — don’t edit. |
| `asgi.py` | For **asynchronous** web servers (e.g., Daphne) | Used in deployment (advanced). |
| `wsgi.py` | For **traditional synchronous** servers (e.g., Gunicorn + Nginx) | Deployment config — ignore for now. |
| `settings.py` | ⭐ **Core config file** | Controls DB, apps, middleware, static files, security, time zone, etc. <br> - Default DB: SQLite <br> - `INSTALLED_APPS`: where you register your apps <br> - `ALLOWED_HOSTS`: required in production |
| `urls.py` (project-level) | ⭐ **Main URL router** | Includes routes → maps URLs to views. <br> Includes `/admin/` by default. |
| `manage.py` | ⭐ **CLI tool for Django commands** | Never edit — use it to run: <br> - `runserver`, `migrate`, `createsuperuser`, `startapp`, etc. |

---

#### 5. **Running the Development Server**
```bash
python manage.py runserver
```
- Starts local server at `http://127.0.0.1:8000`

---

### 🎯 Quick Mental Model
> A **Django project** = one website.  
> A **Django app** = a modular feature/module inside it (e.g., `blog`, `users`, `products`).  
> You’ll create apps *inside* the project using `python manage.py startapp appname`.

---

