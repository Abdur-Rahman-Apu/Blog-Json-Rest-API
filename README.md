# 📝 **Blog REST API using JSON-Server** 🌐

[![JSON-Server](https://img.shields.io/badge/Backend-JSON--Server-ffca28.svg)](https://github.com/typicode/json-server)
[![REST API](https://img.shields.io/badge/API-REST-blue.svg)](https://restfulapi.net/)

Welcome to my **Blog REST API**! This project is built using **JSON-Server**, which mimics a RESTful API for a blogging platform. You can perform CRUD operations on blog posts and author details using various API endpoints.

## 🖥️ **Demo**

🚀 **[Live Demo](https://blog-json-rest-api.onrender.com/)**

---

## 📌 **Features**

- 📝 Manage **blog posts** and **author details**.
- 🔄 Perform **CRUD** operations.
- 🔍 Filter, paginate, and sort results.
- 🗂️ Relationship management between posts and authors.
- 🔧 Built-in query and condition handling.

---

## 🚀 **API Endpoints Overview**

### 🔖 **Posts**

| Endpoint                             | Description                           |
| ------------------------------------ | ------------------------------------- |
| `GET /posts`                         | Fetch all blog posts                  |
| `GET /posts/1`                       | Fetch a single post by ID             |
| `GET /posts?id=1&id=2`               | Fetch posts by multiple IDs           |
| `GET /posts?views_gte=12`            | Fetch posts with views >= 12          |
| `GET /posts?_sort=views&_order=desc` | Sort posts by views (descending)      |
| `GET /posts?_page=1&_limit=5`        | Paginate posts (5 per page)           |
| `GET /posts?category=sports`         | Fetch posts by category (sports)      |
| `GET /posts?title_like=JavaScript`   | Search posts by title (support regex) |
| `GET /posts?_expand=author`          | Include parent author resource        |

### 👤 **Authors**

| Endpoint                    | Description                                    |
| --------------------------- | ---------------------------------------------- |
| `GET /authors`              | Fetch all authors                              |
| `GET /authors?_embed=posts` | Fetch authors along with their posts           |
| `GET /posts?_expand=author` | Fetch posts and expand with the author details |

---

## 🛠️ **API Usage**

### 1. **Fetch All Posts**

```bash
GET http://localhost:3000/posts
```

### 2. **Fetch a Single Post**

```bash
GET http://localhost:3000/posts/1
```

### 3. **Filter Posts Based on Views**

```bash
GET http://localhost:3000/posts?views_gte=12
```

### 4. **Sort Posts by Views in Descending Order**

```bash
GET http://localhost:3000/posts?_sort=views&_order=desc
```

### 5. **Paginate Posts (5 posts per page)**

```bash
GET http://localhost:3000/posts?_page=1&_limit=5
```

---

## 🔗 **Relationship Management**

### **Include Child Resources**

To fetch authors along with their posts:

```bash
GET http://localhost:3000/authors?_embed=posts
```

### **Include Parent Resources**

To fetch posts along with the details of their respective authors:

```bash
GET http://localhost:3000/posts?_expand=author
```

---

## 🌍 **Sorting & Pagination**

You can easily paginate and sort the results:

| Parameter     | Usage                                       |
| ------------- | ------------------------------------------- |
| `_page=1`     | Specifies the page number                   |
| `_limit=5`    | Specifies the number of results per page    |
| `_sort=views` | Sort by the "views" field                   |
| `_order=desc` | Sort in descending order (use with `_sort`) |
| `_order=asc`  | Sort in ascending order (use with `_sort`)  |

---

## 🛠️ **Installation & Setup**

1. Clone the repository:
   ```bash
   git clone https://github.com/Abdur-Rahman-Apu/Blog-Json-Rest-API.git
   ```
2. Install **dependencies**:
   ```bash
   npm install
   ```
3. Run the JSON-Server:

   ```bash
      npm run dev
   ```

4. Access the API at:
   ```bash
   http://localhost:3000
   ```

---

## 🔧 **Tools & Technologies**

- **JSON-Server**: A full fake REST API.
- **REST API**: Standard API architecture.

---

## ⭐ **Request for Star**

If you find this project helpful, please consider giving it a **star** on GitHub to support me!

---

## 📬 **Contact**

- **GitHub**: [Abdur-Rahman-Apu](https://github.com/Abdur-Rahman-Apu)
- **LinkedIn**: [Abdur Rahman Apu](https://www.linkedin.com/in/abdur-rahman-apu)

---
