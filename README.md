# Buyer–Seller OOP System + PostgreSQL Integration

This project is an academic final assignment for the Databases course.  
The system is based on a Buyer–Seller marketplace implemented in Java (OOP), extended with a PostgreSQL database layer.

The code is organized into several components based strictly on the files in the project.

---

## 🧩 Entities (Core Classes)

The following classes represent the core data objects in the system:

- **User** – Base class for system users  
- **Buyer** – Represents a buyer  
- **Seller** – Represents a seller  
- **Product** – Represents a product  
- **ProductSpecialPackage** – Represents a special or bundled product package  
- **Cart** – Represents a buyer’s cart  
- **Address** – Stores user address details  
- **Categories** – Enum for product categories

These classes hold the data for buyers, sellers, products, carts, and addresses.

---

## 🛠️ Management Layer

The system includes manager classes responsible for handling the logic of each entity:

- **ManagerBuyer** – Handles operations related to Buyer  
- **ManagerSeller** – Handles operations related to Seller  
- **ManagerProduct** – Handles operations related to Product  
- **ManagerFacade** – Coordinates operations between all managers  
- **Manageable (interface)** – Defines shared manager behavior

This layer organizes the system functions into clear modules.

---

## 🗄️ Database Layer (PostgreSQL)

The project integrates with a PostgreSQL database through:

- **DBConnection** – Manages the database connection  
- **SQL_HELPER** – Assists with executing SQL queries and updates

These classes enable persistent storage and retrieval of system data.

---

## ⚙️ Utilities & Interfaces

Supporting classes used across the project:

- **ProductInterface** – Interface for product-related behavior  
- **SellerInterface** – Interface for seller-related behavior  
- **UserInput** – Handles system/user inputs  
- **FactoryUser** – Creates Buyer or Seller objects  
- **FactoryProduct** – Creates Product objects

Factories simplify object creation and reduce code duplication.

---

## ▶️ Program Entry Point

- **Main.java**  
  The starting point of the system. Initializes the managers, database connection, and controls the overall flow.

---

## 🎯 Project Purpose

- Implement a Buyer–Seller system using Object-Oriented Programming (OOP) in Java  
- Add PostgreSQL database functionality to store system data  
- Use dedicated manager classes to handle operations for buyers, sellers, and products  
- Utilize JDBC via DBConnection and SQL_HELPER to communicate with the database  
- Maintain a clear modular architecture: entities, managers, utilities, and database layers

---
