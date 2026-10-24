# 🤝 Handoff: Bite & Co. Food Hall

**Date:** June 3, 2026
**Project Folder:** `BiteAndCo/`
**GitHub:** https://github.com/Juwanj32/BiteAndCo

---

## 🎯 The Project
A Java CLI multi-restaurant food hall ordering system demonstrating core OOP principles — abstract classes, inheritance, encapsulation, and polymorphism. Built from scratch as a resume project.

## 📊 Current Status: 95% Complete
- [x] All 3 order types working — Dine In, Delivery, Pickup (100%)
- [x] Cart system working — items add correctly, confirmation prints (100%)
- [x] Order summary working — items listed, totals calculated, prices formatted (100%)
- [x] Service charge and delivery fee applied correctly (100%)
- [x] Price formatting with `String.format("%.2f")` (100%)
- [x] Git initialized, `.gitignore` clean, pushed to GitHub (100%)
- [x] README written and pushed (100%)
- [ ] Input validation — user can enter invalid numbers and crash the app (0%)
- [ ] GUI — JavaFX or Swing (future, not urgent)

## 🗂️ Files
```
BiteAndCo/
├── Main.java            # Entry point — CLI loop and user input
├── order.java           # Abstract parent class
├── dineInOrder.java     # 10% service charge, table number
├── deliveryOrder.java   # $3.99 delivery fee, address
├── pickUpOrder.java     # No extra charge, pickup time
├── Customer.java        # Name, email, phone
└── menuItems.java       # Item name and price
```

## ⚠️ Known Issues
- **VS Code run button is broken** for this project — always compile and run from terminal:
  ```bash
  javac *.java && java Main
  ```
- Input validation is missing — entering a letter instead of a number will throw an `InputMismatchException`

## ⏭️ Next Steps if Returning to This Project
1. Add input validation using `try/catch` around `scanner.nextInt()` calls
2. Consider a JavaFX GUI as a v2 stretch goal

## ✅ Concepts Phil Has Locked In From This Project
- Abstract classes and why you can't instantiate them directly
- Inheritance with `extends` and `super()`
- Polymorphism — same method call, different behavior per subclass
- Encapsulation — private fields, public getters
- `ArrayList` vs fixed arrays and when to use each
- Scanner input and buffer clearing with `scanner.nextLine()`
- `String.format("%.2f")` for decimal formatting
- Git workflow — `add`, `commit`, `push`, `.gitignore`
- `javac *.java && java Main` for multi-file compilation

---
**Current Status:** Project is fully functional and on GitHub. Resume-ready.
