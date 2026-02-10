# 🚁 Drone Delivery Manager – .NET 🚁

![GitHub stars](https://img.shields.io/github/stars/ElyasafCohen100/Drone-Delivery-Manager-dotnet?style=social)
![GitHub forks](https://img.shields.io/github/forks/ElyasafCohen100/Drone-Delivery-Manager-dotnet?style=social)

> **Mini Project | Windows Systems Engineering**  
> A full management system for a drone-based delivery company

---

## 🏷️ Technologies & Tools

### 🖥️ Frontend 🖥️
![WPF](https://img.shields.io/badge/WPF-Desktop_App-0078D6?style=for-the-badge)
![XAML](https://img.shields.io/badge/XAML-UI_Design-0A66C2?style=for-the-badge)

### ⚙️ Backend & Core ⚙️
![C#](https://img.shields.io/badge/C%23-.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-Framework-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)

### 💾 Data & Infrastructure 💾
![XML](https://img.shields.io/badge/XML-Data_Storage-FF8C00?style=for-the-badge)
![Factory Pattern](https://img.shields.io/badge/Factory_Design_Pattern-2E8B57?style=for-the-badge)
![Singleton Pattern](https://img.shields.io/badge/Singleton-Design_Pattern-8A2BE2?style=for-the-badge)

### 🔄 Runtime & Simulation 🔄
![Simulation Engine](https://img.shields.io/badge/Drone_Simulator-Life_Cycle-2496ED?style=for-the-badge)
![BackgroundWorker](https://img.shields.io/badge/BackgroundWorker-Multithreading-3C3C3D?style=for-the-badge)

---

## ✨ Overview ✨

**Drone Delivery Manager** is a desktop application designed to manage a drone delivery company.  
The system supports full management of drones, parcels, customers, and base stations, including a **live drone simulator**.

The project was developed as part of a **Windows Systems Engineering mini project**, with a strong focus on clean architecture, separation of concerns, and proper design patterns.

---

## 🧱 System Architecture 🧱

The project is built using a **3-Layer Architecture**:

- 📁 Presentation Layer (WPF)
- 📁 Business Logic Layer (BL)
- 📁 Data Access Layer (DAL)

### 🔹 Presentation Layer (WPF)
- Graphical user interface
- Two separate interfaces:
  - 👤 **Customer UI**
  - 🛠️ **Admin / Manager UI**

### 🔹 Business Logic Layer (BL)
- Handles all business rules
- Manages drones, parcels, customers, and base stations
- Controls the drone life-cycle simulation

### 🔹 Data Access Layer (DAL)
The DAL is implemented in **two different ways**:

1. **In-Memory Lists**  
   - Data is stored in memory only  
   - All data is lost when the application is closed

2. **XML-Based Storage**  
   - Data is stored persistently in XML files  
   - Data is preserved between application runs

---

## 🏭 Factory Design Pattern 🏭

The system uses the **Factory Design Pattern** to control which DAL implementation is active.

### 🔄 Switching DAL Implementation
1. Open the file:
dal-config.xml

2. Change the **third line** to the desired DAL implementation
3. Restart the application

No code changes are required ✔️

---

## 🪴 User Interfaces 🪴

### 👥 Customer Interface
- View personal parcels 📦
- Create new parcels for delivery 📦

### 🛠️ Admin / Manager Interface
- View and manage:
- 🚁 Drones
- 🧍 Customers
- 🏢 Base Stations
- 📦 Parcels
- Display extended details for each entity
- Run the drone simulator

---

## 🎮 Drone Simulator 🎮

The project includes a **drone life-cycle simulator** that simulates real-world drone behavior.

### ▶️ How to Run the Simulator
1. Log in as **Admin** 🤵
2. Open **Drone List** 📝
3. Select a drone (double click) 🚁
4. Click the **Simulator** button 😇

🌱 The simulator runs using `BackgroundWorker` for smooth UI performance. 🌱

---

## 🔄 XML DAL – Important Note

For smooth usage of the XML-based DAL implementation:

1. Click the **Reset** button on the main window 🔘
2. Close the application 🔒
3. Restart the project 🔄

This prevents data conflicts and ensures clean initialization. 🧴🫧

---

## 🔐 Login Credentials 🔐

### 👤 Customers
- Username: `customer0`, `customer1`, ...
- Password: same as the username

### 🛠️ Admin
- Username: `admin`
- Password: `admin`

### ⚡ VIP Mode
- The **VIP** button allows login without credentials  
- Intended for debugging and development purposes

---

## 🧑‍💻 Contributors 🧑‍💻

- **Yakir Yohanan** 🤘😌 
- **Elyasaf Cohen** 👊😎

[![Yakir Yohanan](https://img.shields.io/badge/GitHub-yohanan400-FF8C00?style=for-the-badge&logo=github&logoColor=white)](https://github.com/yohanan400)  
[![Elyasaf Cohen](https://img.shields.io/badge/GitHub-ElyasafCohen100-0A66C2?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ElyasafCohen100)

---

## 💥 Final Notes 💥

This project demonstrates:
- Clean architecture  
- Strong separation of concerns  
- Proper use of design patterns  
- Practical simulation of real-world delivery systems  

⭐ If you like this project – please leave a star! ⭐  
