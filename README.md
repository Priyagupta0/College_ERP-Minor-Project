# 🎓 College ERP 

A full-stack Django-based College ERP system for managing students, staff, courses, subjects, attendance, notifications, and more. Built with AdminLTE for a responsive and intuitive UI.

---

## 🚀 Features

- Role-based access: Admin, Staff, Student
- Course & Subject management
- Student & Staff CRUD with profile photo uploads
- Attendance tracking with reports
- Push notifications via Firebase Cloud Messaging (FCM)
- Email-based authentication
- Responsive UI using AdminLTE

---

## 🛠 Tech Stack

- **Backend**: Python, Django
- **Database**: SQLite (default) or any Django-supported DB
- **Frontend**: AdminLTE, jQuery, Bootstrap

---

## ⚡ Quick Start (Windows)

1. **Create and activate virtual environment**
   ```bash
   python -m venv venv
   .\venv\Scripts\activate
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   # Or minimally:
   pip install django requests
   ```

3. **Apply migrations**
   ```bash
   python manage.py migrate
   ```

4. **Create superuser**
   ```bash
   python manage.py createsuperuser
   ```

5. **Run development server**
   ```bash
   python manage.py runserver
   ```

6. **Access the app**
   - App: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
   - Admin: [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/)

---

## 📁 Project Structure

```plaintext
College-ERP/
├── main_app/
│   ├── templates/
│   │   ├── main_app/
│   │   │   ├── base.html
│   │   │   ├── footer.html
│   │   │   ├── login.html
│   │   │   └── sidebar_template.html
│   │   └── registration/
│   │       └── base.html
│   ├── static/
│   │   ├── dist/       # AdminLTE assets
│   │   └── plugins/    # AdminLTE plugins
│   ├── views.py
│   ├── hod_views.py
│   └── models.py
├── media/              # Uploaded user images
└── manage.py
```

---

## ⚙️ Configuration Notes

- Static files served from `main_app/static/`
- Uploaded images stored in `media/`
- Google reCAPTCHA included in `login.html` (set your site key for production)
- FCM example code in `views.py` (replace with your API keys)

---

## 🧰 Common Commands

- Make migrations: `python manage.py makemigrations`
- Apply migrations: `python manage.py migrate`
- Create superuser: `python manage.py createsuperuser`
- Run server: `python manage.py runserver`

---

## 📄 License

This project is provided as-is for educational purposes. Consider applying an appropriate license for your use case.
