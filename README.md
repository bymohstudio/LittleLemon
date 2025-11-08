# 🍋 Little Lemon Restaurant Web Application  

A simple **Django REST Framework** project for managing restaurant operations such as menu items, table bookings, and user authentication.  
This project was built as part of the **Meta Back-End Developer Professional Certificate** to demonstrate full-stack and API development skills.  

---

## 🚀 Features  

- 🧾 **Menu Management** – Create, read, update, and delete menu items.  
- 🍽️ **Table Bookings** – Manage restaurant table reservations.  
- 🔐 **User Authentication** – Token-based login and registration.  
- ⚙️ **Admin Panel** – Access and manage all restaurant data easily.  
- 🧩 **Modular Django App Structure** – Clean and maintainable code design.  

---

## 🧠 Tech Stack  

- **Backend:** Django, Django REST Framework  
- **Database:** MySql 
- **Authentication:** Token-based (using DRF’s `authtoken`)  
- **Frontend:** Django templates (optional for testing)  
- **Tools:** Insomnia, Python 3.10+, Git  

---

## 🧭 API Endpoints  

| Endpoint | Description | Methods |
|-----------|--------------|----------|
| `/restaurant/` | Home route | GET |
| `/restaurant/menu/` | Manage menu items | GET, POST |
| `/restaurant/menu/<id>` | Retrieve or modify a specific menu item | GET, PUT, DELETE |
| `/restaurant/booking/tables` | Manage table bookings | GET, POST, PUT, DELETE |
| `/auth/users/` | Register a new user | POST |
| `/auth/token/login/` | Login and obtain authentication token | POST |

---

## ⚙️ Setup Instructions  

1. **Clone the Repository**
   ```bash
   git clone https://github.com/bymohstudio/LittleLemon.git
   cd LittleLemon
