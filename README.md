# turbo_tender

## 📦 Tender Management System – README (Revised)

### 🏗 Overview

The Tender Management System streamlines the complete tender lifecycle—from tender creation and publication to bid submission, evaluation, and award.
It is designed for organizations that need transparency, control, and auditability across procurement activities.

---

### ✨ Features

* 📄 Create and manage tenders
* 👥 Vendor registration & authentication
* 💼 Submit bids securely
* 🧮 Automated or manual bid evaluation
* 🏆 Final award dashboard
* 🗂 Full revision history and audit logs
* 🔐 Role-based access (Admin / Vendor / Reviewer)
* ☁ Deployable on local or cloud infrastructure

---

### 🏛 Tech Stack

* **Backend:** Python (TemperPy Framework)
* **Database:** PostgreSQL / SQLite
* **Auth:** JWT / Session based
* **Optional:** Celery for scheduled job execution (tender deadlines, reminders)

---

### 🚀 Getting Started

#### 1️⃣ Clone the repository

```bash
git clone https://github.com/<org>/tender-management.git
cd tender-management
```

#### 2️⃣ Create a virtual environment and install dependencies

```bash
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

#### 3️⃣ Configure environment variables

Create `.env`:

```
DATABASE_URL=postgres://user:password@localhost:5432/tenders
SECRET_KEY=super-secret
```

#### 4️⃣ Run migrations

```bash
temperpy migrate
```

#### 5️⃣ Start the server

```bash
temperpy runserver
```

App is now available at:

```
http://localhost:8000
```

---

### 🧪 Testing

```bash
pytest
```

---

### 📁 Folder Structure

```
tender-management/
├─ tenders/           # Core tender module
├─ bids/              # Bid lifecycle
├─ users/             # Authentication and roles
├─ utils/             # Shared helpers
└─ config/            # Settings & env
```

---
⚙️ What It Actually Does

Publish. Bid. Evaluate. Award. Audit.
One clean flow:

1️⃣ Admins publish tender details
2️⃣ Vendors submit bids with files & metadata
3️⃣ Reviewers compare & score intelligently
4️⃣ A winner gets crowned (with receipts)
5️⃣ Auditors can trace every click later

All automatic reminders, permissions, and data validation baked in.
### 📌 Roadmap

* Vendor scoring matrix
* Attachment validation & virus scanning
* E-auction add-on
* REST & GraphQL API exposure

---

### 🤝 Contributing

Pull requests are welcome!
Please open an issue before making major changes.

---

### 📄 License

