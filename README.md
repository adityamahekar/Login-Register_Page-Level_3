🔐 Login & Register Page – Level 3 Authentication

This project is a Login & Register Authentication System built with Node.js, Express, EJS, and PostgreSQL.
It demonstrates Level 2 Authentication, where user passwords are salted and hashed using bcrypt.js (Blowfish cipher) before storing them in the database.

Users can register with an email and password, log in securely, and gain access to a protected secrets page.
The project follows a modular EJS structure using partials (header.ejs, footer.ejs) and serves static assets through the public folder.

This is an educational project that shows how to implement scoure authentication and oraganize a full-stack Node.js app.

---

y

## 📷 Gallery

| SignUp Page | Login Page |
|-------------|------------|
| ![al4](./imgg/al4.png) | ![al3](./imgg/al3.png) |

| Register Page | Secret Page |
|---------------|-------------|
| ![al1](./imgg/al1.png) | ![lgl3](./imgg/lgl3.png) |

| Database |
|----------|
| ![al2](./imgg/al2.png) |


---

## ⚙️ Setup Instructions

 1️⃣ Create Table in PostgreSQL(users):
 <br><br>
as given in the query.sql
 <br>
 
2️⃣ Install Dependencies:
```bash
npm i
npm i pg express ejs body-parser
```

3️⃣ Database Connection (index.js)
```bash
const app = express()
const db = new pg.Client({
  user: "postgres",
  host: "localhost",
  database: "XXXXX",    // <-- your database name
  password: "XXXXX",    // <-- your password
  port: XXXX,           // <-- your port name, by default for pg 5432
});
```
4️⃣ Run Server:
```bash
node index.js
```
---
👉 [Open App on Localhost](http://localhost:3000)
