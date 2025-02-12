# API Testing with Postman - Evaluation Project

## 📌 Overview
This project contains API test collections created using **Postman** to evaluate various API endpoints.  
The APIs tested in this collection are based on `https://dummyjson.com`, which provides fake data for testing purposes.

---

## 📂 Collection Details

### ✅ **User Authentication**
- **`POST /auth/login`** - Authenticate user and create a session
- **`GET /auth/me`** - Retrieve user session details  

### ✅ **Product Management**
- **`GET /products`** - Fetch all products  
- **`GET /products/{id}`** - Retrieve details of a single product  
- **`GET /products/search?q=phone`** - Search products based on a keyword  
- **`GET /products?limit=10&skip=10&select=title,price`** - Fetch limited products with specific fields  
- **`GET /products/categories`** - Get all product categories  
- **`GET /products/category/{category-name}`** - Get products of a specific category  
- **`POST /products/add`** - Add a new product  
- **`PUT /products/{id}`** - Update an existing product  
- **`DELETE /products/{id}`** - Delete a product  

---

## ⚙️ Prerequisites
To run the API tests, you need:  
- **Postman** installed on your system  
- **Internet access** to send requests to `https://dummyjson.com`  

---

## 🚀 How to Use  

### 📌 **1. Import the Collection**
1. Open **Postman**
2. Click on **Import**  
3. Upload the provided **evaluation.postman_collection.json** file  

### 📌 **2. Run Requests Manually**
1. Open **Postman**
2. Select any API request  
3. Click **Send** to test the response  

### 📌 **3. Run Automated Tests (Optional)**
- If tests are included in the collection:
  1. Open **Runner** in Postman  
  2. Select the **collection**  
  3. Click **Run**  

---

## 🔍 Expected Responses  

| HTTP Status Code | Meaning |
|-----------------|---------|
| **200 OK** | Successful API request |
| **201 Created** | Resource successfully created |
| **400 Bad Request** | Invalid parameters provided |
| **401 Unauthorized** | Authentication failure |
| **404 Not Found** | Requested resource does not exist |
| **500 Internal Server Error** | Server error |

---

## 🛠️ Sample API Requests  

### **🔹 GET Request Example (Fetch All Products)**
```http
GET https://dummyjson.com/products
