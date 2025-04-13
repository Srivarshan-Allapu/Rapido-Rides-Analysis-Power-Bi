---

# 🛵 Rapido Rides Analysis Dashboard – Power BI

## 📊 Project Overview

This Power BI dashboard provides a detailed analytical view of **Rapido rides data**, covering metrics such as total fare, duration, distance, service usage, cancellation trends, payment methods, and user reviews. The goal is to understand ride patterns, performance by service type, and customer behavior insights to support operational decisions.

---

## 🚀 Key Features

- 📈 **Total Fare Analysis** across services
- ⏱️ **Sum of Duration** & Distance per ride category
- 🚕 **Service Comparison** – Auto, Bike, Bike Lite, Cab Economy, Parcel
- ❌ **Ride Status** – Completed vs. Cancelled
- 💳 **Payment Method Distribution** (Paytm, GPay, QR, Amazon Pay, etc.)
- 💬 **Review Filtering** for successful rides
- 🔍 **Dynamic Filters** for:
  - Service Type
  - Cancellation Reason
  - Reviews

---

## 🧬 Data Model & Source

- **Source**: PostgreSQL (or CSV/Excel if imported manually)
- **Connection**: Import mode (can be adapted to DirectQuery)
- **Tables Used**:
  - `rides`: ride_id, service_type, status, duration, distance, fare, etc.
  - `payments`: ride_id, payment_method
  - `cancellations`: ride_id, cancellation_reason
  - `reviews`: ride_id, review_text, rating

---

## 📂 Folder Structure

```
Rapido-Rides-Analysis/
├── README.md
├── Rapido_Rides_Analysis.pbix
└── Data/
    └── sample_rides_data.csv
    └── schema_description.txt
```

---

## 🧱 Requirements

- Power BI Desktop (latest version)
- PostgreSQL ODBC Driver (if using live connection)
- Rapido rides data in CSV or PostgreSQL
- [Optional] SQL script for PostgreSQL schema setup

---

## ⚙️ Setup Instructions

1. **Clone this repository**  
   Download or clone the dashboard project files.

2. **Open in Power BI Desktop**  
   Launch Power BI and open `Rapido_Rides_Analysis.pbix`.

3. **Connect to your data source**  
   - If using PostgreSQL:
     - Go to `Transform Data` → `Data Source Settings`
     - Update server/database credentials
   - If using CSV:
     - Replace the sample CSV file with your updated data keeping the same schema

4. **Apply Filters & Explore**  
   Interact with slicers and charts to uncover insights by service type, payment mode, or review feedback.

---

## 📸 Dashboard Snapshot

![Screenshot 2025-04-13 194622](https://github.com/user-attachments/assets/5128dfd5-5f65-419e-af6c-74319c0a5dc3)


---

## 📈 Sample KPIs

- **Total Fare**: ₹24.61M
- **Total Duration**: 3.2M seconds
- **Total Rides**: ~50K
- **Most Used Service**: Bike
- **Top Payment Methods**: Paytm, GPay, QR scan

---

## 📌 Use Cases

- Identifying underperforming service types
- Evaluating ride completion vs. cancellation patterns
- Monitoring preferred customer payment behavior
- Optimizing service allocation by distance & duration

---

## 👨‍💻 Author

Developed by [Allapu Srivarshan]  
📧 [allapuramesh68@gmail.com]

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---
