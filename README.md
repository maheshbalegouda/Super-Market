# 🛒 Supermarket Checkout System

A simple and interactive web-based application that calculates the total price of selected items, including applicable discount offers. This is built using Python and Django for backend processing, with a clean and modern UI for user interaction.

---

## 🔍 Features

### 📋 Price List Interface

- A fixed list of products with their **unit prices** and **available discount offers**.
- Discounts are automatically applied during checkout based on item quantity.

| SL No | Item | Unit Price (₹) | Discount Offer      |
|-------|------|----------------|----------------------|
| 1     | A    | 50             | Buy 3 for ₹130       |
| 2     | B    | 30             | Buy 2 for ₹45        |
| 3     | C    | 20             | —                    |
| 4     | D    | 15             | —                    |

---

## 🧾 How It Works

1. **Input Field**  
   Users enter a string representing their items (e.g., `AABBC`).  
   - Each character corresponds to an item.
   - Valid inputs: `A`, `B`, `C`, `D`.

2. **Calculate Total**  
   On clicking the **"Calculate Total"** button, the system:
   - Parses the input string.
   - Applies unit prices and available discounts.
   - Displays the **final total amount**.

3. **Clear Button**  
   Resets the input field and output result.

---

## 💰 Example Calculation

Input: `AABC`  
Breakdown:
- A x2 → ₹50 x 2 = ₹100  
- B x1 → ₹30  
- C x1 → ₹20  
**Total = ₹150**

But if `B` appears twice: `AABBC`  
- A x2 → ₹100  
- B x2 → ₹45 (discount)  
- C x1 → ₹20  
**Total = ₹115**

---

## 📜 Checkout History

Each calculation is stored in the **Checkout History** table with:
- Serial Number
- Items Entered
- Total Price (₹)

This helps track previous transactions during the session.

---

## 🖼️ UI Preview

### 🔹 Price List & Entry
![Price List UI](./path/to/your/image1.png)

### 🔹 Price Calculation & Checkout History
![Checkout Result UI](./path/to/your/image2.png)

---

## 🚀 Technologies Used

- **Frontend:** HTML, CSS, Bootstrap (custom styled)
- **Backend:** Python, Django
- **Storage:** In-memory (session-based)

---

