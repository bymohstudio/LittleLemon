# 🍋 Little Lemon Restaurant Web Application  

A **Django REST Framework** project built for managing a restaurant’s menu, bookings, and user authentication.  
This project demonstrates hands-on skills in **database design**, **API development**, **token authentication**, and **Django ORM** — developed as part of the **Meta Back-End Developer Professional Certificate**.  

---

## 🚀 Features  

- 🧾 **Menu Management** – Add, view, update, and delete menu items.  
- 🍽️ **Table Bookings** – Handle restaurant reservations using CRUD operations.  
- 🔐 **User Authentication** – Token-based login and registration via Djoser.  
- ⚙️ **Admin Panel** – Manage menu and booking data through Django Admin.  
- 🧩 **Modular Architecture** – Organized Django app structure following RESTful design.  

---

## 🧠 Tech Stack  

- **Backend:** Django, Django REST Framework  
- **Database:** SQLite  
- **Authentication:** Token-based (Djoser)  
- **Frontend (optional):** Django templates / Postman for testing  
- **Tools:** Python 3.10+, Git, Postman  

---

## 🧭 API Endpoints  

| Endpoint | Description | Methods |
|-----------|--------------|----------|
| `/restaurant/` | Home route | GET |
| `/restaurant/menu/` | Manage menu items | GET, POST |
| `/restaurant/menu/<id>` | Retrieve or modify a specific menu item | GET, PUT, DELETE |
| `/restaurant/booking/tables` | Manage table bookings | GET, POST, PUT, DELETE |
| `/auth/users/` | Register a new user | POST |
| `/auth/token/login/` | Obtain token for authentication | POST |

---

## ⚙️ Setup Instructions  

1. **Clone the Repository**
   ```bash
   git clone https://github.com/bymohstudio/LittleLemon.git
   cd LittleLemon
   ```

2. **Create and Activate Virtual Environment**
   ```bash
   python -m venv env
   source env/bin/activate  # macOS/Linux
   env\Scripts\activate     # Windows
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run Migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create Superuser (Optional)**
   ```bash
   python manage.py createsuperuser
   ```

6. **Start the Development Server**
   ```bash
   python manage.py runserver
   ```

---

## 🔑 Authentication  

Token-based authentication is enabled using **Djoser**.  

### 🔐 Auth Routes  
- `/auth/users/` → Register new user  
- `/auth/token/login/` → Obtain login token  

### 🧍 Default Admin Credentials  
```
Username: admindjango  
Password: employee@123!
```

---

## 🧪 Example Usage  

### Get Menu Items
```bash
GET /restaurant/menu/
```

### Create a New Booking
```bash
POST /restaurant/booking/tables
```

**Request Body:**
```json
{
  "name": "John Doe",
  "guest_count": 2,
  "booking_date": "2025-11-08T19:30:00Z"
}
```

---

## 🖥️ Admin Panel  

Access the Django admin dashboard to manage all restaurant data:  
👉 [http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin)

---

## 🧩 Project Structure  

```
LittleLemon/
│
├── restaurant/          # Core restaurant app
│   ├── models.py        # Database models
│   ├── views.py         # API logic
│   ├── serializers.py   # Data serialization
│   └── urls.py          # API endpoints
│
├── LittleLemon/         # Main Django project folder
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
└── manage.py
```

---

## 🧾 License  

This project was created for educational purposes as part of the **Meta Back-End Developer Professional Certificate**.  

---

## 👨‍💻 Author  

**Mohit Mishra**  
🎓 Meta Certified Back-End Developer  
🧠 Skilled in Python, Django, DRF, and REST APIs
