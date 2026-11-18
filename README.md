# PeopleHub - HR Employee Self-Service Portal

A small web portal where employees manage their own leave and get quick answers, and admins handle approvals. Built as my final-year B.Sc. IT project.

## Features
- Secure login for employees and admins (hashed passwords, role-based access)
- Employee dashboard with leave balance and leave history
- Apply for leave, with checks on dates, available balance and overlapping leave
- Admin panel to approve or reject requests; balances update automatically
- State-wise leave entitlements
- Leave policy page and a keyword-based HR chatbot (rule-based, not AI)
- Error pages for access denied, page not found and server errors

## Tech stack
Python 3, Flask, SQLite, HTML/CSS (Jinja2 templates)

## How to run
1. Install Python 3 and then Flask: `pip install flask`
2. Run: `python app.py`
3. Open http://127.0.0.1:5000/login in your browser

The database (`peoplehub.db`) is created automatically on first run.

## Sample logins (demo data)
| Role | Email | Password |
|---|---|---|
| Admin | admin@peoplehub.com | admin123 |
| Employee (Maharashtra) | harpreet@example.com | 1234 |
| Employee (Delhi) | priya@example.com | priya123 |

## Screenshots
![Dashboard](screenshots/dashboard.png)
![Apply leave](screenshots/apply-leave.png)
![Admin panel](screenshots/admin.png)

## Project structure
- `app.py` - routes, database setup, leave checks, admin actions, chatbot
- `templates/` - HTML pages
- `static/` - CSS and static files

## Future scope
Attendance tracking, email notifications, password reset, and an AI-based chatbot.

## Note
This is a college project built with sample data. It is not connected to any company's real HR data.
