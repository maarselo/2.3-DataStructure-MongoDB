# 🍃 2.2-MongoDB-Modeling

A complete set of MongoDB database modeling exercises, focusing on Entity–Relationship (ER) diagrams represented as JSON schemas.  
This project demonstrates how to design and structure NoSQL databases for real-world scenarios such as an Optics store, a Food Delivery platform, and a simplified YouTube system.

---

## 📄 Description - Exercise Statement

In this project we model several case studies using **MongoDB collections** instead of SQL relational tables.  
Each exercise includes a **visual ER diagram** (created with [JsonCrack](https://jsoncrack.com)) and an equivalent **JSON schema** that can be imported for visualization.  

The goal is to understand how to translate traditional relational models into **document-oriented databases**, and to practice working with hierarchical structures and relationships in MongoDB.

Deliverables per exercise:
- Diagram file in `.png`
- JSON schema for visualization (no execution required)

---

## 🧾 Level 1

### 👓 Optics Store
We design a two MongoDB schema for the store **“Cul d’Ampolla”** to manage clients and glasses sales.  
The database stores information about:

- **Suppliers**: name, address (street, number, floor, door, city, postal code, country), phone, fax, tax ID.  
- **Glasses**: brand, graduation (left/right lenses), frame type (floating, pasta, metallic), frame color, lenses color, price.  
- **Clients**: name, address, phone, email, registration date, and who recommended them.  
- **Employees**: track which employee sold each pair of glasses.  
- **Sales**: date/time of transaction.

---

## 🍴 Level 2

### 🍕 Food Delivery Platform
We design a schema for an online food delivery system.  
The database stores:

- **Clients**: ID, name, surname, address, postal code, city, province, phone.  
- **Orders**: ID, date/time, type (delivery/pickup), products (type, quantity), total price, notes.  
- **Products**: pizzas, burgers, drinks. Includes ID, name, description, image, price. Pizzas have categories that change over time.  
- **Stores**: ID, address, postal code, city, province.  
- **Employees**: ID, name, surname, NIF, phone, role (cook/delivery).  

Relations modeled:  
- One client → many orders.  
- One store → many orders.  
- One employee → one store.
- One order → many products.   
- Orders can be assigned to delivery employees with delivery date/time.  

---

## 🎦 Level 3

### Simplified YouTube
We design a simplified YouTube-like schema.  
The database stores:

- **Users**: ID, email, password, username, birthdate, gender, country, postal code.  
- **Videos**: ID, title, description, size, filename, duration, thumbnail, views, likes, dislikes, status (public, hidden, private).  
- **Tags**: multiple tags per video.  
- **Channels**: ID, name, description, creation date.  
- **Subscriptions**: users subscribing to channels.  
- **Likes/Dislikes**: tracked per user with timestamp.  
- **Playlists**: ID, name, creation date, status (public/private).  
- **Comments**: ID, text, timestamp, related user & video.  

Relations modeled:  
- One user → many videos.  
- One user → many playlists.  
- One video → many tags. 
- One user → one channel.
- One user → many comments.  
- Users can subscribe to other users’ channels.  

---

## 💻 Technologies Used
- Database bases: MongoDB  
- Diagram Tool: JsonCrack  

---

## 📋 Requirements
Before reviewing this project, make sure you:  
- Open the **JSON files** in JsonCrack to visualize schemas.  
- Open the **.png diagrams** for quick reference.  

> ⚠️ No execution is required. The JSON files are only for visualization.

---

## 🛠️ Installation
1. Clone the repository. 
2. Open the `.json` files in JsonCrack or any JSON viewer.  
3. Open the `.png` diagrams for the ER structure.  

---

## ▶️ Running the Project
- There is **no execution required** since this project is focused on **data modeling**.  
- Simply open the diagrams and JSON schemas to review the database structures.  

---

## 🌐 Deployment
Not applicable. The project is only for design and visualization purposes.  

---

## 🤝 Contributions
Suggestions to improve schemas or alternative modeling strategies are welcome.  
Feel free to propose additional improves to JSON structures.  

---

## 🙏 **Thank you for reviewing this project!** 🚀  
