<p align="center">
  <img src="https://github.com/user-attachments/assets/d3981340-deb4-4e4b-aac3-b9a112947524" alt="favicon" width="139" height="195" />
</p>

<h1 align="center"><b>BillSwift 💸</b></h1>
  
Smart Billing & Invoice Manager for Small Businesses
BillSwift is a desktop-based billing system built to simplify day-to-day invoicing, tax calculation, and bill management for small and medium businesses.
It focuses on:
- Fast bill creation
- Reliable storage using a local database
- Professional PDF invoice export
- Simple admin-only access
Features
- 🧾 Create & Manage Bills
  - Add customer details, product items, quantities, discounts, and taxes
  - Auto-calculated totals (subtotal, tax, discount, grand total)
- 👨‍💼 Admin Login System
  - Secure login screen for admin
  - Only authenticated users can create or view bills
- 📚 Bill History & Search
  - View all past bills
  - Search bills by:
    - Bill number
    - Customer name
    - Date range
- 📄 PDF Generation
  - Generate professional-looking PDF invoices
  - Easy to share/print for customers or accounting
- 🗃 SQLite Database Storage
  - All bills, products, customers, and bill items are stored safely in a local SQLite database
  - No external server required
- 🏬 Product Management
  - Store commonly sold products
  - Quickly add them to any bill
- 💰 Discounts & Taxes
  - Per-bill or per-item discount handling (based on your logic)
  - Configurable tax percentage (e.g., GST)
---
 🧱 Tech Stack
- Language: Python 3.x  
- GUI Framework: Tkinter (or your chosen GUI framework)  
- Database: SQLite3  
- PDF Generation: (e.g., `reportlab` / `fpdf` – update based on your project)  
---
📂 Project Structure
```bash
BillSwift/
├── main.py               # Entry point of the application
├── db/
│   ├── bills.db          # SQLite database
│   └── migrations.sql    # (If any) DB schema or setup script
├── src/
│   ├── ui/               # GUI-related modules (windows, dialogs, components)
│   ├── models/           # Database models / data access logic
│   ├── services/         # Billing, PDF, and business logic
│   └── utils/            # Helper functions, constants, validators
├── assets/
│   ├── logo.png          # App logo / icons
│   └── templates/        # PDF templates, if used
├── requirements.txt      # Python dependencies
└── README.md
```

#⚙️ Installation
### 1️⃣ Clone the Repository

```bash
git clone https://github.com/karthikrapolu17/BillSwift.git
cd BillSwift
```

### 2️⃣ Create a Virtual Environment (Recommended)

```bash
python -m venv venv
# Windows
venv\Scripts\activate
# Linux / macOS
source venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```
---
##  Running the Application

```bash
python main.py
```
Once the app starts:
1. Log in using the admin credentials (default can be something like `admin/admin123` if configured).
2. Navigate to **New Bill** to create a bill.
3. Add customer and product details.
4. Apply discounts/taxes as needed.
5. Save the bill.
6. Export as **PDF** if required.
---
## 🗄 Database Overview
BillSwift uses SQLite to store all data locally. Typical tables (may vary based on your implementation):
- `users` – admin credentials and roles  
- `customers` – customer details  
- `products` – product catalog  
- `bills` – main bill header (customer, date, totals)  
- `bill_items` – line items linked to each bill  
---
## 🛣️ Roadmap / Future Improvements
Planned or potential enhancements:
- Multi-user roles (e.g., cashier, manager)
- GST-compliant invoice formats
- Product stock/inventory management
- Export reports to Excel/CSV
- Cloud backup / sync option
- Dark mode UI
---
 🤝 Contributing
Contributions, issues, and feature requests are welcome!
1. Fork the repository  
2. Create your feature branch:  
   ```bash
   git checkout -b feature/awesome-feature
   ```
3. Commit your changes:  
   ```bash
   git commit -m "Add awesome feature"
   ```
4. Push to the branch:  
   ```bash
   git push origin feature/awesome-feature
   ```
5. Open a Pull Request
---
## 📄 License
This project is licensed under the **MIT License**.

