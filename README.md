# EduCycle — Sustainable Resale Platform for Engineering Students

EduCycle is a web-based peer-to-peer marketplace exclusively for university campuses, enabling students and staff to **buy, sell, and exchange** second-hand academic materials like textbooks, electronics, stationery, and more in a trusted, eco-friendly environment.

---

## Overview

Generic platforms like OLX or eBay are not designed for campus communities — they lack trust, campus focus, and essential academic-use features. EduCycle solves this with a dedicated platform that promotes:

- **Affordability** — Buy and sell used goods at fair prices
-  **Trust** — Verified profiles, reviews, and admin moderation
-  **Sustainability** — Reduce waste by reusing academic resources
-  **Community** — Connect buyers and sellers directly on campus

---

## Project Structure

```
eduCycleEcommerce/
│
├── public/                  # Static assets
├── docs/                    # Project documentation
├── src/
│   ├── ai/                  # AI-related utilities
│   ├── app/                 # Next.js app router pages
│   ├── components/          # Reusable UI components
│   ├── contexts/            # React context providers
│   ├── data/                # Static/mock data
│   ├── hooks/               # Custom React hooks
│   ├── lib/                 # Utility functions
│   └── products/
│       └── new/             # New product listing flow
├── .gitignore
├── apphosting.yaml
├── components.json
└── README.md
```

---

## Features

### Role-Based Access
Three distinct user roles — **Buyer**, **Seller**, and **Admin** — each with their own dashboard and permissions.

### Buyer Features
- Browse and search listings with advanced filters (category, price range, condition)
- Add to Cart or Wishlist
- Checkout with a transparent 5% platform fee
- View purchase history

### Seller Features
- Create product listings with images, description, price, and condition
- Manage and edit/delete existing listings
- View sales analytics dashboard

### Want to Buy (WTB) Board
- Post requests for specific items with a budget
- Sellers can directly respond to buyer requests

### Admin Panel
- User management — view, verify, suspend, or delete accounts
- Platform reports — revenue overview, sales history, analytics
- Monitor all transactions and platform activity

### FAQ Page
- Separate sections for Buyers and Sellers
- Covers platform fees, listing rules, and WTB board usage

---

## Architecture

The platform follows a **4-layer web architecture**:

| Layer | Technology |
|---|---|
| Presentation Layer | React.js (Next.js) + Browser Storage |
| Application Layer | Node.js API + JWT Authentication |
| Business Layer | User roles and transaction logic |
| Data Layer | React Context + Local Storage |

---

## Process Flow

1. **Authentication** — User registers/logs in and is assigned a role (Buyer / Seller / Admin)
2. **Product Listing** — Sellers create listings with images, price, category, and condition
3. **Discovery** — Buyers search and filter products; browse or use WTB Board
4. **Transaction** — Add to Cart → Checkout → 5% platform fee applied → Confirm Purchase
5. **Administration** — Admin verifies accounts, monitors sales, and manages the platform

---

## Tech Stack

| Technology | Purpose |
|---|---|
| Next.js (React) | Frontend framework |
| Tailwind CSS | Styling |
| React Context API | State management |
| Browser Local Storage | Persistent data storage |
| JWT | User authentication |
| Node.js | Backend API |

---

## Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/Akanksha11-S/eduCycleEcommerce.git
cd eduCycleEcommerce

# 2. Install dependencies
npm install

# 3. Run the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---
