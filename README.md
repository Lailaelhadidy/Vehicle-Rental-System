# Vehicle Rental System (Java)

## 📌 Overview
The **Vehicle Rental System** is a console-based Java application developed as part of a university **Object-Oriented Programming (OOP)** project.  
It simulates a real-world vehicle rental environment using advanced OOP concepts.

---

## 🎯 Core Idea
The system manages:
- Different types of vehicles (Car, Bike, Bus)
- Customers
- Vehicle rental and return operations

Each vehicle type follows its own pricing strategy, demonstrating runtime polymorphism.

---

## ⚙️ Features
- Add new vehicles (Car, Bike, Bus)
- Register customers
- List all vehicles and customers
- Rent vehicles to customers
- Return rented vehicles
- Prevent duplicate IDs
- Menu-driven console interface

---

## 🧱 System Design

### Main Components
- **Vehicle (Abstract Class)**
- **Car, Bike, Bus (Subclasses)**
- **Rentable (Interface)**
- **Customer**
- **RentalManager**
- **Main Program**

---

## 📘 Class Descriptions

### Vehicle (Abstract Class)
**Fields:**
- `vehicleID`
- `model`
- `basePricePerDay`
- `rented`
- `rentedBy`

**Methods:**
- `isRented()`
- `setRented()`
- `getRentedBy()`
- `calculatePrice(int days)` *(abstract)*
- `toString()`

---

### Rentable (Interface)
**Methods:**
- `rent(int days, Customer c)`
- `returnVehicle()`

---

### Car
- Extends `Vehicle`
- Adds number of seats
- Overrides pricing logic

---

### Bike
- Extends `Vehicle`
- Implements unique pricing logic

---

### Bus
- Extends `Vehicle`
- Adds passenger capacity
- Custom price calculation

---

### RentalManager
**Static Fields & Methods**
- Manages vehicles and customers
- Handles renting and returning logic
- Centralized system control

---

## 🧠 OOP Concepts Demonstrated
- Abstraction
- Inheritance
- Polymorphism
- Interfaces
- Encapsulation
- Static Variables & Methods
- Arrays and Loops
