Book My Stay App:

**Version:** 1.0  
**Author:** Dishita D
**GitHub:** https://github.com/Dishiitaa0607/Bookmystayapp

Project Overview:

The Book My Stay App is a **Hotel Booking Management System** developed in **Core Java** using fundamental **data structures**.  
The project demonstrates real-world software challenges like inventory consistency, fair request handling, and prevention of double-booking.  

It is developed incrementally through multiple **Use Cases (UCs)**, each introducing a new concept while reinforcing previous ones.

Project Structure:
BookMyStayApp/
│
├── src/
│ ├── UseCase1HotelBookingApp.java
│ ├── UseCase2RoomInitialization.java
│ ├── UseCase3InventorySetup.java
│ ├── UseCase4RoomSearch.java
│ └── ... (additional UCs if implemented)
│
├── README.md
└── .git/ (git repository)

Use Case Summary:

| UC | Name | Goal | Key Concepts |
|----|------|------|--------------|
| UC1 | Application Entry & Welcome Message | Demonstrate program startup and console output | `class`, `main()` method, `static`, `System.out.println()` |
| UC2 | Basic Room Types & Static Availability | Introduce object-oriented domain modeling | `abstract class`, inheritance, polymorphism, encapsulation |
| UC3 | Centralized Room Inventory Management | Maintain inventory consistently using a data structure | `HashMap`, single source of truth, encapsulation |
| UC4 | Room Search & Availability Check | Allow guests to view available rooms without changing inventory | Read-only access, defensive programming, separation of concerns |

Installation & Setup:

1. **Clone the repository**
```bash
git clone https://github.com/Dishiitaa0607/Bookmystayapp.git
cd Bookmystayapp/src

javac UseCase1HotelBookingApp.java
javac UseCase2RoomInitialization.java
javac UseCase3InventorySetup.java
javac UseCase4RoomSearch.java


---

Git Workflow Used:

- **Main branches**
  - `main` → production-ready code
  - `develop` → integration branch

- **Feature branches**
  - `feature/UC1`, `feature/UC2`, etc.

- **Workflow**
  1. Create feature branch from `develop`
  2. Code and test UC
  3. Commit and push feature branch
  4. Merge into `develop`
  5. Delete feature branch after merge (optional)

- **Commands used**
```bash
git checkout develop
git checkout -b feature/UCx
git add .
git commit -m "UCx: feature description"
git push -u origin feature/UCx
git checkout develop
git merge feature/UCx
git push
git branch -d feature/UCx
git push origin --delete feature/UCx

---

Key Learnings:

- Proper separation of **read-only vs write operations**
- Centralized state management with `HashMap`
- Incremental development using **feature branches**
- Avoiding double-booking and inconsistent data
- Incremental object-oriented design: abstract classes, inheritance, polymorphism

Improvements:

- Add **user input** to allow dynamic room booking
- Implement **real-time concurrency** handling for multiple guests
- Introduce **GUI or Web interface** for better usability
- Extend inventory with **amenities, booking history, pricing strategies**

Conclusion:

This project demonstrates **practical use of Java and data structures** to implement a scalable hotel booking system.  
By working through incremental use cases, the system showcases **robust design, maintainability, and real-world software engineering practices**.
