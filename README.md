# Retro Video Game Store App

## 📦 Overview

The **Retro Video Game Store App** is a multi-component project that simulates a full-featured game rental and purchase platform. Developed for the Enterprise Application Development course, the application allows users to browse and rent classic GameBoy Advance (GBA) titles, track shipping status, and earn rewards for their activity.

The solution integrates:
- A **Python Console Client** for user interaction
- A **Web-based Shipping Tracker** built with ASP.NET MVC
- A **Backend API** developed with ASP.NET Core and Entity Framework
- A centralized **SQL Server database** for users, games, orders, and rewards

---

## 🚀 Features

- **User Login & Account Management**  
  Sign up to rent games and auto-fill shipping info in future orders.

- **Game Rental System**  
  Browse from a curated GBA collection and place orders easily.

- **Order Tracking**  
  Check delivery status directly from the Shipping Tracker interface.

- **Rewards System**  
  Earn points for every rental, track them, and redeem them later.

---

## 🧱 Architecture

The solution is composed of 5 main projects:

1. **GameStoreApp** – Front-end (future planned)
2. **GameStoreAPI** – Core API (ASP.NET Core)
3. **GameStoreData** – Data layer with shared models and migrations
4. **GameShippingTracker** – ASP.NET MVC web app for shipping tracking
5. **GameStoreClient.py** – Python console client for user actions

### 📊 Database Entities
- **Users** – Login info, linked orders, rewards
- **Games** – Title, genre, release date, price, stock
- **Orders** – User orders, status, quantity, total
- **Rewards** – Tracks user-earned points
- **ShippingInfo** – Delivery address and tracking details

---

## 🔐 Security

- The API uses **basic authentication** via a custom `AuthenticationHandler`.
- Default credentials:  
  `admin / password`  
  (future expansion to individual user auth supported)

---

## 🧪 Testing

- **Postman** used for automated endpoint testing
- Validated all CRUD operations for:
  - Users
  - Games
  - Orders
  - Rewards

---

## 💻 Running the Project

### Python Client
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
2. Run the application:
   python GameStoreClient.py

### ASP.NET Web App
1. Open EADProject.sln in Visual Studio.
2. Build and run the GameStoreApp project.
3. Access the app in your browser at https://localhost:7219
