# ✍️ ProBlog: Multi-Role Blogging Engine
**A production-ready Django blogging system featuring granular access control, dynamic dashboards, and robust media management.**

[![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)](https://www.djangoproject.com/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)

---

## 🌟 Overview
ProBlog is not just a simple blogging site; it's a **Role-Based Content Management System (CMS)**. It mimics real-world production environments where different users (Admins, Managers, Editors, and Authors) have specific permissions and dedicated dashboards to manage content efficiently.

### ✨ Key Features
* **🔐 Multi-Role Authorization:** Custom permission logic using Django Groups for Admin, Manager, Editor, and Author roles.
* **📊 Role-Specific Dashboards:** Custom views for Editors and Managers with real-time data counts and management tables.
* **📝 Advanced CRUD:** Full lifecycle for Posts and Categories with unique slug generation and automated media handling.
* **💬 Engagement System:** Secure comment section restricted to authenticated users.
* **🔍 Intelligent Search:** Full-text search functionality that retains search terms across paginated results.
* **🛡️ Security & Auth:** Robust user registration, login/logout flows, and decorator-based view protection.

---

## 🛠️ Tech Stack
| Component | Technology |
| :--- | :--- |
| **Framework** | Django 4.x (Python 3.10+) |
| **Database** | PostgreSQL / MySQL / SQLite |
| **Frontend** | Django Templates, HTML5, CSS3 |
| **Auth** | Django Contrib Auth (Groups & Permissions) |
| **Storage** | Media & Static file handling for Image uploads |

---

## 📂 Architecture
```text
blog_project/
├── core/               # Project settings & WSGI
├── blog/               # Main application logic (Models, Views, Slugs)
├── users/              # Authentication & Profile management
├── templates/          # Role-specific Dashboards & Blog layouts
├── static/             # Assets (CSS, JS, Images)
├── media/              # User-uploaded post covers
└── manage.py
