# Recipe App Backend

A lightweight RESTful API built using **Express.js** and **PostgreSQL** to support the Recipe Mobile App. This backend handles recipe data, categories, favorites, and integrates with Clerk authentication.

---

## Features

* Express.js REST API
* PostgreSQL database
* Clerk user authentication middleware
* CRUD for Recipes & Categories
* Favorites system (save/remove)
* Environment-based configuration

---

## Tech Stack

* **Node.js + Express**
* **PostgreSQL**
* **Drizzle ORM**
* **JWT / Clerk Auth**
* **Dotenv** for environment variables

---

##  Environment Variables

Create `.env` file:

```
DATABASE_URL=postgresql://username:password@localhost:5432/recipe_db
PORT=5001
CLERK_SECRET_KEY=your-secret-key
```

---

##  Installation & Setup

### 1. Install dependencies

```
npm install
```

### 2. Run database migration (if any)

```
npx drizzle-kit migrate
```

### 3. Start server

```
npm run dev
```

Server will run on:

```
http://localhost:5001
```

---

## Authentication

Protected routes use Clerk verification middleware:

```
Authorization: Bearer <token>
```



## 📄 License

This project is license
