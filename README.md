# 📦 Stock Inventory System

An **Excel-based inventory management system** for tracking stock credits and debits and viewing the net stock of every item. It uses formulas and a macro-driven **Update** button to log transactions, so item names, credit and debit totals, and net quantities are all calculated automatically.

![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?logo=microsoftexcel&logoColor=white)
![VBA](https://img.shields.io/badge/VBA-Macros-blue)
![Format](https://img.shields.io/badge/Format-.xlsm-green)
![Type](https://img.shields.io/badge/Type-Self%20Project-lightgrey)

---

## 📑 Table of Contents

- [Features](#-features)
- [How It Works](#-how-it-works)
- [Quick Start](#-quick-start)
- [How to Use](#-how-to-use)
- [Repository Contents](#-repository-contents)
- [Important Notes](#-important-notes)
- [Author](#-author)

---

## ✨ Features

- 📋 Central item list with unique item codes and names
- ➕ Simple entry of stock credits (additions) and debits (removals)
- 🔽 Item code dropdown fed from the item list, and item names filled in automatically
- 🧮 Net stock per item calculated automatically
- ⚡ Macro-enabled **Update** button to log each transaction
- 🔗 Consistent data across all worksheets

---

## 🧩 How It Works

The workbook has three worksheets that feed into each other.

| Worksheet | Role |
|-----------|------|
| **Items List** | The master list of item codes and names, used by the other sheets |
| **Sheet1** (Inventory Management Log Book) | Where you record every stock transaction |
| **Net Stock** | Summary of credits, debits, and the current quantity per item |

```text
Items List ──► Sheet1 (log book) ──► Net Stock
 (codes, names)   (credits, debits)     (net quantity)
```

**Formulas used:** `VLOOKUP` to fetch item names, `IF` to split a quantity into the Credited or Debited column, and `SUMIFS` to total each item's transactions.

---

## ⚡ Quick Start

1. Download `Update and Count.xlsm` from this repository.
2. Open it in **Microsoft Excel** and click **Enable Content** or **Enable Macros** when prompted.
3. Add your items to **Items List**.
4. Log transactions in **Sheet1** and click **Update**.
5. Open **Net Stock** to see current quantities.

---

## 📋 How to Use

### 1. Update the item list (**Items List**)

Add each product with a unique **Item Code** and an **Item Name**. The other sheets use this list, so keep it current.

| Item Code | Item Name |
|-----------|-----------|
| 4001 | Product A |
| 4002 | Product B |

### 2. Record transactions (**Sheet1**)

| Field | How to fill it |
|-------|----------------|
| **Item Code** | Pick from the dropdown (populated from the Items List) |
| **Item Name** | Filled in automatically with `VLOOKUP` |
| **Type** | Choose **Credited** (stock added) or **Debited** (stock removed) |
| **Quantity** | Number of items |
| **Date** | Transaction date |

The quantity is placed in the **Credited** or **Debited** column according to the type. Then click **Update** to run the macro, which adds the transaction as a new row in the log.

### 3. View net stock (**Net Stock**)

- Item codes and names are pulled from the Items List.
- Total credits and debits for each item are summed from Sheet1.
- **Net quantity = Credited − Debited.**
- The sheet recalculates whenever Sheet1 changes.

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `Update and Count.xlsm` | The macro-enabled inventory workbook |
| `Manual.pdf` | User manual (PDF) |
| `Manual.ipynb` | User manual (notebook) |
| `how to use.html` | User manual (HTML) |

---

## 📝 Important Notes

- **Macros must be enabled** for the **Update** button to work.
- Keep the **Items List** accurate, because the dropdowns and the Net Stock sheet depend on it.
- The workbook needs Microsoft Excel for full macro support.

---

## 👤 Author

**Siddharth Acharya**
B.E. Computer Engineering, Himalaya College of Engineering (HCOE), Tribhuvan University
GitHub: [@acharya-2226](https://github.com/acharya-2226)

Open for educational and personal use. Feel free to adapt it for your own learning or inventory needs.
