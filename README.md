# Inventory Management System

**Developed by Rachit Sapkota & Team**

## Overview
The Inventory Management System (IMS) is a comprehensive web application designed for small to medium-sized businesses to efficiently manage inventory, sales, and overall operations. It combines modern frontend and backend technologies to deliver performance, scalability, and security. The system allows real-time inventory tracking, user management with role-based access, invoice generation, and insightful reporting, all through an intuitive interface.

## Features
- **Inventory Management:** Add, edit, remove, and categorize products with details such as SKU, stock quantity, price, and supplier information. Real-time updates prevent overstock or shortages.
- **Sales & Invoice Generation:** Record sales transactions and generate clean, printable PDF invoices for professional billing.
- **User Roles & Security:** Admin, Manager, and Staff roles with JWT-based authentication and encrypted passwords.
- **Reports & Dashboard:** Visualize stock levels, sales trends, and low-stock alerts. Export reports for auditing and decision-making.
- **Self-Hosted Deployment:** Run on your own server using Node.js and MongoDB for full control over data and operations.

## Tech Stack
- **Frontend:** React.js + TailwindCSS
- **Backend:** Node.js + Express
- **Database:** MongoDB
- **PDF Generation:** react-pdf

## Folder Structure
```
inventory-management-system/
├─ backend/          # Server-side logic, routes, controllers, models, and config
├─ frontend/         # React frontend components, pages, and utilities
├─ invoices/         # Invoice templates for PDF generation
├─ README.md         # Setup guide and documentation
├─ package.json      # Project dependencies
└─ .env.example      # Environment variables example
```

## Setup Instructions
### 1. Clone Repository
```bash
git clone https://github.com/yourusername/inventory-management-system.git
cd inventory-management-system
```

### 2. Backend Setup
```bash
cd backend
npm install
cp .env.example .env
# Edit .env with MongoDB URI and JWT secret
node app.js
```

### 3. Frontend Setup
```bash
cd frontend
npm install
npm start
```

### 4. Access Application
Open your browser and navigate to `http://localhost:3000`.

### 5. Create Invoice
- Navigate to Sales > Create Invoice
- Enter customer and product details
- Download or print PDF invoice

### 6. Deploy on Server
- Ensure Node.js and MongoDB are installed
- Configure Nginx/Apache as a reverse proxy
- Enable HTTPS for secure connections
- Start backend and serve frontend build

## Security Recommendations
- Use strong passwords and secure JWT keys
- Regularly back up the database
- Monitor server logs and enable firewalls

This project is fully populated, production-ready, and optimized for self-hosted deployment.
