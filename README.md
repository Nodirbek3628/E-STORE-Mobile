# 🛒 FINAL EXAM PROJECT

## **Cyber Store – E-Commerce Backend API**

### 🎯 Maqsad:

Talabaning **real E-Commerce backend loyiha** ustida ishlash ko‘nikmalarini baholash:

* REST API dizayn
* Authentication & Authorization (JWT, Permission)
* Business Logic & Validation
* Performance (ORM optimizatsiya)
* E-Commerce flow (Cart, Order, Payment)
* API hujjatlashtirish

---

## 1️⃣ TEXNOLOGIYALAR (MAJBURIY)

* Python 3.x
* Django
* Django Rest Framework (DRF)
* JWT Authentication (`djangorestframework-simplejwt`)
* PostgreSQL
* Swagger / Redoc (`drf-spectacular`)
* `.env` (environment variables)
* Git + GitHub (public repository)

---

## 2️⃣ FOYDALANUVCHI ROLLARI

| Role      | Tavsif                                      |
| --------- | ------------------------------------------- |
| **Admin** | Tizim va mahsulotlarni boshqaradi           |
| **User**  | Mahsulot sotib oladi, buyurtma beradi       |

---

## 3️⃣ MA’LUMOTLAR MODELLARI

### 👤 User (Custom User)

```text
id
username
email
password
is_active
created_at
