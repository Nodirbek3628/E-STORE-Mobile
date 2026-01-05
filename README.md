# 🛒 PROJECT

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
```
### 📦 Category
```text
id
name
slug
created_at
```
### 📱 Product
```
id
category (FK)
name
brand
price
discount_price
description
stock
rating
created_at
```
### 🖼 ProductImage
```
id
product (FK)
image
```
### ❤️ Wishlist
```
id
user (FK)
product (FK)
created_at
```
### 🛒 Cart
```
id
user (OneToOne)
updated_at
```
### 🛍 CartItem
```
id
cart (FK)
product (FK)
quantity

```
### 📦 Order
```
id
user (FK)
total_price
status (pending / paid / cancelled)
created_at

```
### 📦 OrderItem

```
id
order (FK)
product (FK)
price
quantity

```
### 💳 Payment

```
id
order (FK)
payment_method
payment_status
transaction_id
created_at

```
### ⭐ Review
```
id
user (FK)
product (FK)
rating (1–5)
comment
created_at

```




