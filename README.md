# 🍔 Bite & Co. Food Hall

A robust, console-based multi-restaurant food hall ordering system built in Java. **Bite & Co.** simulates a real-world dining platform that handles multiple order types (Dine-In, Delivery, and Pickup), dynamic cart management, automated fee calculations, and polymorphic order processing.

Designed and developed from scratch as a portfolio project to demonstrate core Computer Science and Object-Oriented Programming (OOP) principles.

---

## 🚀 Key Features

* **Polymorphic Order Processing:** Leverages abstract classes and method overriding to handle unique business logic (such as service charges and delivery fees) dynamically based on the chosen fulfillment type.
* **Unified Cart & Dynamic Pricing:** Allows items to be added to a centralized cart, automatically calculating sub-totals, service fees, or delivery charges with precise decimal formatting (`String.format("%.2f")`).
* **Flexible Fulfillment Options:** 
  * *Dine-In:* Automatically calculates and applies a 10% service charge linked to specific table numbers.
  * *Delivery:* Applies a flat delivery fee and captures delivery addresses.
  * *Pickup:* Processes standard pickup orders with scheduled times[cite: 1].
* **Robust Data Structures:** Utilizes `ArrayList` collections for efficient item tracking and order summary generation.

---

## 🛠️ Tech Stack & Concepts

* **Language:** Java
* **Core OOP Principles:** 
  * *Abstraction:* Using abstract parent classes (`order.java`) to define shared structures[cite: 1].
  * *Inheritance:* Extending base functionality into specialized subclasses (`dineInOrder`, `deliveryOrder`, `pickUpOrder`)[cite: 1].
  * *Polymorphism:* Executing uniform method calls that behave differently depending on the runtime object type.
  * *Encapsulation:* Protecting internal state via private fields and public getter/setter methods.
* **Development Tools:** Git, GitHub, VS Code / Terminal CLI[cite: 1].

---

## 🗂️ Project Structure

```text
BiteAndCo/
├── Main.java            # Entry point — CLI execution loop and user input handling
├── order.java           # Abstract parent class defining core order properties
├── dineInOrder.java     # Subclass handling 10% service charge and table numbers
├── deliveryOrder.java   # Subclass handling $3.99 delivery fees and addresses
├── pickUpOrder.java     # Subclass handling pickup scheduling
├── Customer.java        # Encapsulates customer details (name, email, phone)
└── menuItems.java       # Manages individual item names and prices
