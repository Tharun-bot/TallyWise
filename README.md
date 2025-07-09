# TallyWise — Web-Based Tally & Ledger Management System

TallyWise is a full-stack web-based accounting and ledger management system inspired by traditional Tally software. It offers a modern interface and a robust backend for managing ledgers, vouchers, and generating comprehensive financial reports.

## Features

- Role-based access control with JWT authentication (Admin, Accountant, Viewer)
- Ledger creation and management
- Voucher entry for Payment, Receipt, Contra, and Journal types
- Automated generation of Trial Balance, Profit & Loss Statement, and Balance Sheet
- Import/export functionality using CSV files
- PDF generation of financial reports
- Clean and responsive frontend interface

## Tech Stack

**Frontend**
- React.js
- Bootstrap

**Backend**
- Django
- Django REST Framework
- PostgreSQL
- JWT authentication (`djangorestframework-simplejwt`)

**Utilities**
- `pandas` for CSV handling
- `xhtml2pdf` or `WeasyPrint` for PDF generation

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Node.js 18 or higher
- PostgreSQL

### Backend Setup

```bash
cd backend
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

# Configure your PostgreSQL database and environment variables

python manage.py migrate
python manage.py runserver
