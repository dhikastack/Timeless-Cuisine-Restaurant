# Timeless-Cuisine-Restaurant

## Overview

A system analysis and design project for **Timeless Cuisine Restaurant**, an Indonesian restaurant serving dine-in and take-away services.

The project focuses on designing an integrated system to improve **ordering, payment, inventory, procurement, supplier management, and reporting** processes.

**Tools:**
-
Figma: https://www.figma.com/design/c8TA2axgRvmsxm5IS80CZC/ISAD-Timeless-Cuisine-Restaurant?node-id=0-1&t=zIKiafpTHCeUIe3Q-1
-
Draw.io (UML)

---

## Problem

The existing restaurant processes still face several issues:

- Manual inventory input can cause stock discrepancies.
- Menu availability is not updated in real time.
- Customers have limited options for order preferences.
- Dine-in and take-away selections are not flexible per item.
- Procurement and inventory processes are not fully integrated.
- Sales, stock, and financial data are not centralized.
- Management does not have a real-time dashboard for monitoring.

---

## Proposed Solution

An integrated **Restaurant Information System** that connects:

**Ordering → Payment → Inventory → Procurement → Supplier → Reporting**

The system is designed to provide real-time data synchronization, improve stock management, support flexible ordering, and provide centralized information for management.

---

## System Analysis & Design

### Fishbone Diagram

Identifying the root causes of operational, customer experience, inventory, procurement, and management problems.

<img width="1552" height="2587" alt="fishbone timeless" src="https://github.com/user-attachments/assets/160569ba-8606-4dde-889f-35d34644ae7d" />


### Data Flow Diagram

Illustrating the flow of information between customers, staff, suppliers, payment providers, and the restaurant system.

<img width="883" height="661" alt="dfd context timeless" src="https://github.com/user-attachments/assets/0c2ce077-9c7e-4c5b-9f78-5ac642dcc2cc" />


### Use Case Diagram

Defining system interactions between customers, cashiers, administrators, warehouse staff, purchasing staff, and management.

<img width="2211" height="6270" alt="use case and desc timeless" src="https://github.com/user-attachments/assets/2717e2e0-d9c2-41cf-b824-ea3b5d19727a" />


### Class Diagram

Modeling the main entities and relationships within the system, including orders, payments, menus, ingredients, suppliers, and procurement.

<img width="1037" height="686" alt="class diagram timeless" src="https://github.com/user-attachments/assets/46236ed8-d152-4b3a-8154-33fb56a2f99f" />

### Sequence Diagram

Describing interactions between users and system components throughout key business processes.

<img width="1692" height="4082" alt="sequence timeless" src="https://github.com/user-attachments/assets/c5bf8334-dd4e-4874-8b22-ab7a16d92986" />


### State Transition Diagram

Representing the lifecycle and status changes of key processes such as orders, payments, inventory, and procurement.

<img width="2302" height="1312" alt="std timeless" src="https://github.com/user-attachments/assets/9f98586f-d486-4d0e-8073-16ef2d5a072a" />


---

## Client / Server Architecture

The proposed system uses a simple **three-tier client-server architecture**:

```text
Client
├── Customer Tablet
├── Cashier
├── Staff
└── Manager Dashboard
        ↓
Application Server
├── Order Management
├── Payment
├── Inventory
├── Procurement
├── Supplier Management
└── Reporting
        ↓
Database
└── MySQL / PostgreSQL
