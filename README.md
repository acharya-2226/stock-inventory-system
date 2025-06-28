# 📦 Inventory Management System (Self Project)

This is a robust **Excel-based Inventory Management System** designed and developed as a self project. It enables efficient tracking of stock, credits, debits, and provides real-time inventory summaries using automated calculations and macros.

> 📊 **B.E. Computer Engineering Project by Siddharth**

---

## 🚀 Features

- Centralized item list with unique codes and names
- Simple data entry for stock credits and debits
- Automatic calculation of net stock for each item
- Macro-enabled updates for seamless workflow
- Real-time summary of inventory status
- Consistent data across all worksheets

---

## 🧩 System Structure

The system consists of three main worksheets:

1. **Sheet2: Item List** – Core of stock management
2. **Sheet1: Data Entry** – Record stock transactions
3. **Sheet3: Net Stock Summary** – View current inventory

---

## 📋 How to Use

### 1. Update Item List (**Sheet2**)

- Add new items by entering a unique **Item Code** and **Item Name**.
- This list is referenced throughout the system for consistency.

**Example:**

| Item Code | Item Name  |
|-----------|------------|
| 4001      | Product A  |
| 4002      | Product B  |

---

### 2. Record Transactions (**Sheet1**)

- **Item Code:** Select from dropdown (populated from Sheet2).
- **Item Name:** Auto-filled via VLOOKUP.
- **Type:** Choose **Credit** (add stock) or **Debit** (remove stock).
- **Quantity:** Enter the number of items.
- **Date:** Specify transaction date.

**After entry:** Click the **Update** button to run the macro and log the transaction.

---

### 3. View Net Stock (**Sheet3**)

- **Item Codes/Names:** Auto-populated from Sheet2.
- **Total Credits/Debits:** Summed from Sheet1 transactions.
- **Net Quantity:** Calculated as **Credited – Debited** for each item.
- **Automatic Updates:** Sheet3 reflects all changes instantly.

---

## ⚡ Quick Start

1. **Enable Macros:** Allow macros when opening the file for full functionality.
2. **Add Items:** Enter new products in Sheet2.
3. **Log Transactions:** Use Sheet1 to record stock movements.
4. **Check Inventory:** View up-to-date net stock in Sheet3.

---

## 📝 Important Notes

- Keep **Sheet2** updated for accurate dropdowns and reporting.
- All calculations and summaries are automated—no manual computation needed.
- Macros must be enabled for the **Update** button to work.

---

## 👨‍💻 Author

- **Project by:** Siddharth
- **Program:** B.E. Computer Engineering

---

## 📜 License

This project is open-source and intended for educational and personal use. You may adapt or extend it for your own learning or inventory needs.

---

## 🙏 Acknowledgments

Thanks to all mentors and peers for their support and feedback during the development of this project.
