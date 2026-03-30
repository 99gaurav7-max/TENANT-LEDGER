# 🏠 Tenant Management System

A lightweight, real-time **tenant and rent management dashboard** built using **HTML, JavaScript, and Supabase**.

Designed for property owners to efficiently manage:

* Tenants
* Groups (rooms)
* Transactions
* Monthly reports

---

## 🚀 Features

### 📊 Dashboard & KPIs

* Total Groups
* Active / Inactive Tenants
* Expected vs Collected Rent
* Pending Rent calculation

---

### 👥 Tenant Management

* Add new tenants with:

  * Name, phone, security deposit
  * Group allocation
* Deactivate tenants (move-out handling)
* Delete inactive tenants
* Filter tenants by:

  * Group
  * Status (Active / Inactive)

---

### 🏢 Group Management

* Create groups (A–Z system)
* Assign monthly rent per group
* Update group rent anytime

---

### 💰 Transaction Management

* Record payments:

  * Room Rent
  * Electricity Bill
  * Water Bill
* Multiple payment modes:

  * UPI, Cash, Bank Transfer, Card, etc.
* Filter transactions by:

  * Group
  * Tenant
  * Date range
  * Bill type
  * Payment mode
* Pagination support for large datasets

---

### 📄 PDF Reports

#### 1. Monthly Report

* Group-wise payment summary
* Tenant-wise breakdown
* Active / Inactive status included
* Clean tabular format

#### 2. Transactions Report

* Exports **filtered or full transaction data**
* Sorted: Latest → Oldest
* Includes:

  * Tenant, Group, Bill Type
  * Payment mode
  * Amount breakdown
* Displays **applied filters in report header**

---

## 🧠 Key Concepts Implemented

* Real-time data sync using **Supabase**
* Client-side filtering & pagination
* Dynamic PDF generation using:

  * `jsPDF`
  * `jspdf-autotable`
* State-based UI updates
* Clean modular JavaScript functions

---

## 🛠️ Tech Stack

* **Frontend:** HTML, CSS, JavaScript
* **Backend / Database:** Supabase
* **PDF Generation:** jsPDF + AutoTable

---

## 📂 Project Structure

```
├── index.html        # Login page
├── dashboard.html    # Main dashboard
├── script (inline)   # All JS logic inside dashboard.html
```

---

## 🔐 Authentication

* Handled via **Supabase Auth**
* Users must log in before accessing dashboard
* Each user manages their own property data

---

## ⚙️ Setup Instructions

1. Clone the repository:

   ```bash
   git clone <your-repo-link>
   ```

2. Open `index.html` in browser

3. Configure your Supabase credentials inside:

   ```js
   supabase.createClient("YOUR_URL", "YOUR_KEY")
   ```

---

## 📌 Current Limitations

* Tenant status is binary:

  * Active / Inactive
* No “temporary leave” state (planned improvement)
* Rent expectation is group-based (not tenant-based)

---

## 🔮 Future Improvements

* Add “On Leave” tenant status
* Advanced analytics dashboard
* Export to Excel/CSV
* Mobile app version
* Role-based access (multi-owner system)

---

## 💡 Use Case

Ideal for:

* PG owners
* Rental property managers
* Small-scale landlords

---

## 👨‍💻 Author

Built with focus on **practical usability and real-world scenarios**.

---

## ⭐ If you found this useful

Give it a ⭐ on GitHub — helps visibility and motivation!
