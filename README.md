# Tourzina-Manual-Testing
Manual testing of a live e-commerce ticketing platform — 104 bugs across 5 dashboards
# 🐛 Tourzina — Manual Testing Project

Comprehensive manual testing of **Tourzina** (dev.tourzina.com), a live e-commerce ticketing platform for tours and activities in Egypt. Testing covered 5 dashboards across functional, security, UI/UX, and performance categories.

---

## 📌 Project Overview

| Field | Details |
|---|---|
| **Application Under Test** | Tourzina — E-commerce Ticketing Platform |
| **Environment** | dev.tourzina.com |
| **Testing Type** | Manual / Exploratory Testing |
| **Dashboards Covered** | Website, Admin, Partner, Staff, Supplier |
| **Total Bugs Found** | 104 |
| **Tester** | Ahmed Salah |
| **Test Period** | April – May 2026 |

---

## 📊 Bug Summary

| Severity | Count |
|---|---|
| 🔴 Critical | 22 |
| 🟠 High | 68 |
| 🟡 Medium | 11 |
| 🟢 Low | 3 |
| **Total** | **104** |

| Status | Count |
|---|---|
| Open | 58 |
| In Review | 30 |
| Resolved | 10 |
| Rejected | 6 |

---

## 🖥️ Dashboards Tested

| Platform | Bugs Found |
|---|---|
| Website | 65 |
| Admin Dashboard | 12 |
| Partner Dashboard | 8 |
| Staff Dashboard | 7 |
| Supplier Dashboard | 12 |

---

## 🔍 Bug Categories

### 🔐 Security & RBAC (Role-Based Access Control)
Critical security flaws found across all dashboards:
- Banned/blocked users still able to login and book tickets
- Supplier account active after admin ban/freeze
- Affiliate can request payouts (should be read-only)
- Affiliate can cancel/confirm bookings (should be read-only)
- Supplier can publish reviews (should be read-only)
- Content Creator Support exposes admin and all user tickets
- Session persists after clearing cookies
- Login fields retain credentials after login
- Email accepted as password during signup
- Signup accepts temporary/disposable email addresses
- Missing email ownership verification during sign-up
- Mass account creation abuse possible

### ⚙️ Functional
- Voucher download not working
- Ticket voucher missing QR code
- Cart not updated after checkout
- Cart deletes previous tickets when adding new destination
- Date filter returns all bookings instead of filtered results
- Admin cannot create/edit missions in Rewards & Vouchers Console
- Multiple users can book same in-progress ticket (no locking)
- User can order more tickets than admin availability limit
- Password reset link leads to error page
- Delete account feature not working
- Change password feature not working

### 🎨 UI/UX
- No confirmation when ticket added to cart
- No loading indicator during login
- Duplicate calendar widgets on booking page
- Reviews carousel scrolls too fast — unreadable
- Welcome text cut off in landscape orientation
- Wishlist shows same image for all tickets
- English punctuation misaligned in Arabic interface

### 📱 Checkout & Cart
- Cannot reduce/edit ticket quantity in cart
- Cart emptied after login during checkout
- Checkout session lost after language change
- Checkout progress lost after page refresh
- Checkout flow resets to ticket selection on back

---

## 📁 Repository Structure

```
Tourzina-Manual-Testing/
│
├── Tourzina_Bug_Report.xlsx     # Full bug report with 4 analysis sheets
└── README.md                    # Project documentation
```

### Excel File Contents
| Sheet | Description |
|---|---|
| **Summary** | Auto-calculated dashboard — totals, severity breakdown, status counts, resolution rate |
| **Bug Log** | All 104 bugs with full details — steps, expected, actual, severity, platform |
| **By Module** | Bug count per module broken down by severity |
| **By Platform** | Bug count per dashboard broken down by status |

---

## 🧰 Testing Approach

- **Exploratory Testing** — Unscripted testing across all user roles and flows
- **Functional Testing** — Core flows: signup, login, booking, checkout, voucher, cart
- **Security Testing** — RBAC validation, session handling, input validation
- **UI/UX Testing** — Responsiveness, layout, feedback messages, accessibility
- **Role-Based Testing** — Tested as Website User, Admin, Partner, Staff, Supplier, Affiliate, Content Creator

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Browser DevTools | Console error checking, network monitoring |
| Tourzina Bug Reporter | Bug submission and tracking |
| Microsoft Excel | Bug report documentation |
| GitHub | Version control and portfolio hosting |

---

## 👤 About the Tester

**Ahmed Salah** — ISTQB CTFL v4 certified QA Engineer with experience in manual testing, automation (Playwright + TypeScript), and security/RBAC testing. Trilingual: Arabic (Native), English (B2), German (B2).

🔗 [LinkedIn](https://linkedin.com/in/ahmad-salah-a33319351) | [GitHub](https://github.com/ahmasalah1-droid)
