# 🚗 Parking Lot System in Java

An **advanced, console-based Parking Lot System** built using **Java and Object-Oriented Programming (OOP)** principles.  
This project simulates a real-world parking lot with **time-based parking fees**, **different parking spot sizes**, and **fast vehicle lookup using HashMap**.

Perfect for **Java beginners → intermediate learners**, **college mini-projects**, and **interview preparation**.

---

## ✨ Features

✅ Park and remove vehicles  
✅ Parking fee calculation based on parking duration  
✅ Time tracking using `LocalDateTime`  
✅ Supports different vehicle types (Bike, Car)  
✅ Different parking spot sizes (SMALL, MEDIUM, LARGE)  
✅ Automatic spot allocation based on vehicle size  
✅ Fast O(1) vehicle lookup using `HashMap`  
✅ Clean, scalable OOP design  

---

## 🧠 System Design (OOP)

### Core Components
- **Vehicle (Abstract Class)**
- **Car, Bike (Inheritance)**
- **ParkingSpot**
- **ParkingLot**
- **Enums** for type safety
- **Main** (Driver class)

---

## 🏗️ Class Diagram (Logical)

```
Vehicle (abstract)
├── Bike
└── Car

ParkingLot
├── List<ParkingSpot>
└── HashMap<VehicleNumber, ParkingSpot>

ParkingSpot
├── SpotSize
├── Vehicle
└── EntryTime
```

---

## 📦 Technologies Used

- Java (JDK 8+)
- OOP Concepts
- Collections Framework
- Date & Time API

---

## 🧩 Concepts Covered

- Abstraction
- Inheritance
- Polymorphism
- Encapsulation
- Enums
- HashMap
- Time-based calculations
- Real-world system design

---

## 🚀 How It Works

1. Vehicle arrives at parking lot
2. System finds a suitable parking spot based on size
3. Entry time is recorded
4. Vehicle is stored in a HashMap for fast access
5. On exit:
   - Parking duration is calculated
   - Fee is generated
   - Spot is freed

---

## 💰 Parking Fee Logic

- Minimum charge: **1 hour**
- Fee calculation:
      Parking Fee = Hours Parked × Rate per Hour
- Uses `Duration.between(entryTime, exitTime)`

---

## ▶️ How to Run

1. Clone the repository
 ```bash
 git clone https://github.com/yogeshkumarsaini/parking-lot-system-java.git
```
2. Open in IDE (IntelliJ / Eclipse / VS Code)
3. Compile and run Main.java

---

## 📂 Project Structure

```css
src/
 ├── Bike.java
 ├── Car.java
 ├── Vehicle.java
 ├── ParkingSpot.java
 ├── ParkingLot.java
 ├── SpotSize.java
 ├── VehicleType.java
 └── Main.java
```
---
## 🔮 Future Enhancements

- Multi-floor parking lot
- Dynamic pricing (weekend/night rates)
- Parking tickets
- Database integration
- REST API using Spring Boot
- Unit tests (JUnit)
