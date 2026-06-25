# ScanRemind

ScanRemind is a QR-based reminder web app built with Flask. Users can scan a QR code, open a reminder form, set a date and time, and receive an email reminder when it is due.

The app does not require account creation. Users can manage their reminders using email-based OTP verification.

## Why I built this

I built ScanRemind to practice full-stack Flask development, database handling, QR code generation, background scheduling, and transactional email delivery in a real-world workflow.

## How it works

A user scans the QR code and is taken to a reminder form. After submitting a title, description, email, date, time, and repeat option, the reminder is saved in the database.

A background scheduler checks for due reminders and sends an email notification at the scheduled time.

Users can also manage their reminders by verifying their email with a one-time password.

## Features

- QR code landing page
- Create reminders with title, description, date, and time
- One-time, daily, weekly, and monthly repeat options
- Email reminder delivery using Brevo
- OTP-based reminder management
- View and delete reminders
- SQLite database for local development
- Flask Blueprints for organized routing
- Background reminder checking using APScheduler

## Tech Stack

- Python
- Flask
- SQLite
- HTML/CSS
- Jinja2
- APScheduler
- Brevo Transactional Email API
- QRCode Python package
- python-dotenv
