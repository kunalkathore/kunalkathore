# 🚀 MERN Full Stack Project

![MERN Stack](https://img.shields.io/badge/Stack-MERN-61DAFB?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Tech Stack](#-tech-stack)
- [Folder Structure](#-folder-structure)
- [Prerequisites](#-prerequisites)
- [Installation & Setup](#-installation--setup)
- [Environment Variables](#-environment-variables)
- [Running the Project](#-running-the-project)
- [API Endpoints](#-api-endpoints)
- [Features](#-features)
- [Screenshots](#-screenshots)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📌 Project Overview

Yeh ek **Full Stack Web Application** hai jo **MERN Stack** (MongoDB, Express.js, React.js, Node.js) par build ki gayi hai. Is project mein complete frontend aur backend integration hai jisme user authentication, REST API, aur database management shamil hai.

---

## 🛠 Tech Stack

| Layer      | Technology          |
|------------|---------------------|
| Frontend   | React.js, Axios, React Router DOM |
| Backend    | Node.js, Express.js |
| Database   | MongoDB, Mongoose   |
| Auth       | JWT (JSON Web Token), bcryptjs |
| Styling    | CSS / Tailwind CSS  |
| Dev Tools  | Nodemon, dotenv, cors |

---

## 📁 Folder Structure

```
mern-project/
│
├── client/                   # React Frontend
│   ├── public/
│   └── src/
│       ├── components/       # Reusable Components
│       ├── pages/            # Page Components
│       ├── context/          # Context API / State Management
│       ├── utils/            # Helper Functions
│       ├── App.js
│       └── index.js
│
├── server/                   # Node + Express Backend
│   ├── config/
│   │   └── db.js             # MongoDB Connection
│   ├── controllers/          # Route Logic
│   ├── middleware/           # Auth & Error Middleware
│   ├── models/               # Mongoose Schemas
│   ├── routes/               # API Routes
│   └── server.js             # Entry Point
│
├── .env                      # Environment Variables
├── .gitignore
├── package.json              # Root package (for scripts)
└── README.md
```

---

## ✅ Prerequisites

Shuru karne se pehle, ensure karein ki aapke system mein yeh installed hain:

- [Node.js](https://nodejs.org/) (v18+)
- [npm](https://www.npmjs.com/) ya [yarn](https://yarnpkg.com/)
- [MongoDB](https://www.mongodb.com/) (Local ya Atlas)
- [Git](https://git-scm.com/)

---

## ⚙️ Installation & Setup

### 1. Repository Clone Karein

```bash
git clone https://github.com/your-username/mern-project.git
cd mern-project
```

### 2. Backend Dependencies Install Karein

```bash
cd server
npm install
```

### 3. Frontend Dependencies Install Karein

```bash
cd ../client
npm install
```

---

## 🔐 Environment Variables

Root directory mein `.env` file banayein aur ye variables add karein:

```env
# Server
PORT=5000
NODE_ENV=development

# MongoDB
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/mydb

# JWT
JWT_SECRET=your_super_secret_key
JWT_EXPIRE=7d

# Client URL (for CORS)
CLIENT_URL=http://localhost:3000
```

> ⚠️ **Note:** `.env` file ko kabhi bhi GitHub par push mat karein. Yeh `.gitignore` mein already add honi chahiye.

---

## ▶️ Running the Project

### Development Mode (Backend + Frontend alag alag)

**Backend chalayein:**
```bash
cd server
npm run dev
```

**Frontend chalayein (naye terminal mein):**
```bash
cd client
npm start
```

### Single Command se dono chalayein (Root level se)

```bash
# Root mein package.json mein concurrently setup hona chahiye
npm run dev
```

- 🌐 **Frontend:** `http://localhost:3000`
- 🔧 **Backend API:** `http://localhost:5000`

---

## 📡 API Endpoints

### Auth Routes — `/api/auth`

| Method | Endpoint           | Description         | Auth Required |
|--------|--------------------|---------------------|---------------|
| POST   | `/api/auth/register` | Naya user register  | ❌            |
| POST   | `/api/auth/login`    | User login          | ❌            |
| GET    | `/api/auth/me`       | Current user info   | ✅            |
| POST   | `/api/auth/logout`   | Logout              | ✅            |

### User Routes — `/api/users`

| Method | Endpoint           | Description         | Auth Required |
|--------|--------------------|---------------------|---------------|
| GET    | `/api/users`         | Sabhi users         | ✅ (Admin)    |
| GET    | `/api/users/:id`     | User by ID          | ✅            |
| PUT    | `/api/users/:id`     | User update         | ✅            |
| DELETE | `/api/users/:id`     | User delete         | ✅ (Admin)    |

---

## ✨ Features

- ✅ User Registration & Login (JWT Authentication)
- ✅ Password Hashing (bcryptjs)
- ✅ Protected Routes (Frontend + Backend)
- ✅ REST API with Express.js
- ✅ MongoDB ke saath Mongoose ODM
- ✅ React Router DOM ke saath SPA Navigation
- ✅ Responsive Design
- ✅ Error Handling Middleware
- ✅ CORS Configuration
- ✅ Environment Variables Support

---

## 📸 Screenshots

> Yahan apne project ke screenshots add karein

| Page        | Preview |
|-------------|---------|
| Home Page   | ![Home](#) |
| Login Page  | ![Login](#) |
| Dashboard   | ![Dashboard](#) |

---

## 🤝 Contributing

Contributions welcome hain! Agar aap contribute karna chahte hain:

1. Repository ko **Fork** karein
2. Apni feature branch banayein: `git checkout -b feature/amazing-feature`
3. Changes commit karein: `git commit -m 'Add amazing feature'`
4. Branch push karein: `git push origin feature/amazing-feature`
5. **Pull Request** open karein

---

## 📄 License

Yeh project [MIT License](LICENSE) ke under licensed hai.

---

## 👨‍💻 Author

**Your Name**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: [your-linkedin](https://linkedin.com/in/your-linkedin)
- Email: your.email@example.com

---

<div align="center">
  ⭐ Agar yeh project helpful laga toh <strong>Star</strong> zaroor dein!
</div>
# 🚀 MERN Full Stack Project

![MERN Stack](https://img.shields.io/badge/Stack-MERN-61DAFB?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Tech Stack](#-tech-stack)
- [Folder Structure](#-folder-structure)
- [Prerequisites](#-prerequisites)
- [Installation & Setup](#-installation--setup)
- [Environment Variables](#-environment-variables)
- [Running the Project](#-running-the-project)
- [API Endpoints](#-api-endpoints)
- [Features](#-features)
- [Screenshots](#-screenshots)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📌 Project Overview

Yeh ek **Full Stack Web Application** hai jo **MERN Stack** (MongoDB, Express.js, React.js, Node.js) par build ki gayi hai. Is project mein complete frontend aur backend integration hai jisme user authentication, REST API, aur database management shamil hai.

---

## 🛠 Tech Stack

| Layer      | Technology          |
|------------|---------------------|
| Frontend   | React.js, Axios, React Router DOM |
| Backend    | Node.js, Express.js |
| Database   | MongoDB, Mongoose   |
| Auth       | JWT (JSON Web Token), bcryptjs |
| Styling    | CSS / Tailwind CSS  |
| Dev Tools  | Nodemon, dotenv, cors |

---

## 📁 Folder Structure

```
mern-project/
│
├── client/                   # React Frontend
│   ├── public/
│   └── src/
│       ├── components/       # Reusable Components
│       ├── pages/            # Page Components
│       ├── context/          # Context API / State Management
│       ├── utils/            # Helper Functions
│       ├── App.js
│       └── index.js
│
├── server/                   # Node + Express Backend
│   ├── config/
│   │   └── db.js             # MongoDB Connection
│   ├── controllers/          # Route Logic
│   ├── middleware/           # Auth & Error Middleware
│   ├── models/               # Mongoose Schemas
│   ├── routes/               # API Routes
│   └── server.js             # Entry Point
│
├── .env                      # Environment Variables
├── .gitignore
├── package.json              # Root package (for scripts)
└── README.md
```

---

## ✅ Prerequisites

Shuru karne se pehle, ensure karein ki aapke system mein yeh installed hain:

- [Node.js](https://nodejs.org/) (v18+)
- [npm](https://www.npmjs.com/) ya [yarn](https://yarnpkg.com/)
- [MongoDB](https://www.mongodb.com/) (Local ya Atlas)
- [Git](https://git-scm.com/)

---

## ⚙️ Installation & Setup

### 1. Repository Clone Karein

```bash
git clone https://github.com/your-username/mern-project.git
cd mern-project
```

### 2. Backend Dependencies Install Karein

```bash
cd server
npm install
```

### 3. Frontend Dependencies Install Karein

```bash
cd ../client
npm install
```

---

## 🔐 Environment Variables

Root directory mein `.env` file banayein aur ye variables add karein:

```env
# Server
PORT=5000
NODE_ENV=development

# MongoDB
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/mydb

# JWT
JWT_SECRET=your_super_secret_key
JWT_EXPIRE=7d

# Client URL (for CORS)
CLIENT_URL=http://localhost:3000
```

> ⚠️ **Note:** `.env` file ko kabhi bhi GitHub par push mat karein. Yeh `.gitignore` mein already add honi chahiye.

---

## ▶️ Running the Project

### Development Mode (Backend + Frontend alag alag)

**Backend chalayein:**
```bash
cd server
npm run dev
```

**Frontend chalayein (naye terminal mein):**
```bash
cd client
npm start
```

### Single Command se dono chalayein (Root level se)

```bash
# Root mein package.json mein concurrently setup hona chahiye
npm run dev
```

- 🌐 **Frontend:** `http://localhost:3000`
- 🔧 **Backend API:** `http://localhost:5000`

---

## 📡 API Endpoints

### Auth Routes — `/api/auth`

| Method | Endpoint           | Description         | Auth Required |
|--------|--------------------|---------------------|---------------|
| POST   | `/api/auth/register` | Naya user register  | ❌            |
| POST   | `/api/auth/login`    | User login          | ❌            |
| GET    | `/api/auth/me`       | Current user info   | ✅            |
| POST   | `/api/auth/logout`   | Logout              | ✅            |

### User Routes — `/api/users`

| Method | Endpoint           | Description         | Auth Required |
|--------|--------------------|---------------------|---------------|
| GET    | `/api/users`         | Sabhi users         | ✅ (Admin)    |
| GET    | `/api/users/:id`     | User by ID          | ✅            |
| PUT    | `/api/users/:id`     | User update         | ✅            |
| DELETE | `/api/users/:id`     | User delete         | ✅ (Admin)    |

---

## ✨ Features

- ✅ User Registration & Login (JWT Authentication)
- ✅ Password Hashing (bcryptjs)
- ✅ Protected Routes (Frontend + Backend)
- ✅ REST API with Express.js
- ✅ MongoDB ke saath Mongoose ODM
- ✅ React Router DOM ke saath SPA Navigation
- ✅ Responsive Design
- ✅ Error Handling Middleware
- ✅ CORS Configuration
- ✅ Environment Variables Support

---

## 📸 Screenshots

> Yahan apne project ke screenshots add karein

| Page        | Preview |
|-------------|---------|
| Home Page   | ![Home](#) |
| Login Page  | ![Login](#) |
| Dashboard   | ![Dashboard](#) |

---

## 🤝 Contributing

Contributions welcome hain! Agar aap contribute karna chahte hain:

1. Repository ko **Fork** karein
2. Apni feature branch banayein: `git checkout -b feature/amazing-feature`
3. Changes commit karein: `git commit -m 'Add amazing feature'`
4. Branch push karein: `git push origin feature/amazing-feature`
5. **Pull Request** open karein

---

## 📄 License

Yeh project [MIT License](LICENSE) ke under licensed hai.

---

## 👨‍💻 Author

**Your Name**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: [your-linkedin](https://linkedin.com/in/your-linkedin)
- Email: your.email@example.com

---

<div align="center">
  ⭐ Agar yeh project helpful laga toh <strong>Star</strong> zaroor dein!
</div># 🚀 MERN Full Stack Project

![MERN Stack](https://img.shields.io/badge/Stack-MERN-61DAFB?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Tech Stack](#-tech-stack)
- [Folder Structure](#-folder-structure)
- [Prerequisites](#-prerequisites)
- [Installation & Setup](#-installation--setup)
- [Environment Variables](#-environment-variables)
- [Running the Project](#-running-the-project)
- [API Endpoints](#-api-endpoints)
- [Features](#-features)
- [Screenshots](#-screenshots)
- [Contributing](#-contributing)
- [License](#-license)

---

## 📌 Project Overview

Yeh ek **Full Stack Web Application** hai jo **MERN Stack** (MongoDB, Express.js, React.js, Node.js) par build ki gayi hai. Is project mein complete frontend aur backend integration hai jisme user authentication, REST API, aur database management shamil hai.

---

## 🛠 Tech Stack

| Layer      | Technology          |
|------------|---------------------|
| Frontend   | React.js, Axios, React Router DOM |
| Backend    | Node.js, Express.js |
| Database   | MongoDB, Mongoose   |
| Auth       | JWT (JSON Web Token), bcryptjs |
| Styling    | CSS / Tailwind CSS  |
| Dev Tools  | Nodemon, dotenv, cors |

---

## 📁 Folder Structure

```
mern-project/
│
├── client/                   # React Frontend
│   ├── public/
│   └── src/
│       ├── components/       # Reusable Components
│       ├── pages/            # Page Components
│       ├── context/          # Context API / State Management
│       ├── utils/            # Helper Functions
│       ├── App.js
│       └── index.js
│
├── server/                   # Node + Express Backend
│   ├── config/
│   │   └── db.js             # MongoDB Connection
│   ├── controllers/          # Route Logic
│   ├── middleware/           # Auth & Error Middleware
│   ├── models/               # Mongoose Schemas
│   ├── routes/               # API Routes
│   └── server.js             # Entry Point
│
├── .env                      # Environment Variables
├── .gitignore
├── package.json              # Root package (for scripts)
└── README.md
```

---

## ✅ Prerequisites

Shuru karne se pehle, ensure karein ki aapke system mein yeh installed hain:

- [Node.js](https://nodejs.org/) (v18+)
- [npm](https://www.npmjs.com/) ya [yarn](https://yarnpkg.com/)
- [MongoDB](https://www.mongodb.com/) (Local ya Atlas)
- [Git](https://git-scm.com/)

---

## ⚙️ Installation & Setup

### 1. Repository Clone Karein

```bash
git clone https://github.com/your-username/mern-project.git
cd mern-project
```

### 2. Backend Dependencies Install Karein

```bash
cd server
npm install
```

### 3. Frontend Dependencies Install Karein

```bash
cd ../client
npm install
```

---

## 🔐 Environment Variables

Root directory mein `.env` file banayein aur ye variables add karein:

```env
# Server
PORT=5000
NODE_ENV=development

# MongoDB
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/mydb

# JWT
JWT_SECRET=your_super_secret_key
JWT_EXPIRE=7d

# Client URL (for CORS)
CLIENT_URL=http://localhost:3000
```

> ⚠️ **Note:** `.env` file ko kabhi bhi GitHub par push mat karein. Yeh `.gitignore` mein already add honi chahiye.

---

## ▶️ Running the Project

### Development Mode (Backend + Frontend alag alag)

**Backend chalayein:**
```bash
cd server
npm run dev
```

**Frontend chalayein (naye terminal mein):**
```bash
cd client
npm start
```

### Single Command se dono chalayein (Root level se)

```bash
# Root mein package.json mein concurrently setup hona chahiye
npm run dev
```

- 🌐 **Frontend:** `http://localhost:3000`
- 🔧 **Backend API:** `http://localhost:5000`

---

## 📡 API Endpoints

### Auth Routes — `/api/auth`

| Method | Endpoint           | Description         | Auth Required |
|--------|--------------------|---------------------|---------------|
| POST   | `/api/auth/register` | Naya user register  | ❌            |
| POST   | `/api/auth/login`    | User login          | ❌            |
| GET    | `/api/auth/me`       | Current user info   | ✅            |
| POST   | `/api/auth/logout`   | Logout              | ✅            |

### User Routes — `/api/users`

| Method | Endpoint           | Description         | Auth Required |
|--------|--------------------|---------------------|---------------|
| GET    | `/api/users`         | Sabhi users         | ✅ (Admin)    |
| GET    | `/api/users/:id`     | User by ID          | ✅            |
| PUT    | `/api/users/:id`     | User update         | ✅            |
| DELETE | `/api/users/:id`     | User delete         | ✅ (Admin)    |

---

## ✨ Features

- ✅ User Registration & Login (JWT Authentication)
- ✅ Password Hashing (bcryptjs)
- ✅ Protected Routes (Frontend + Backend)
- ✅ REST API with Express.js
- ✅ MongoDB ke saath Mongoose ODM
- ✅ React Router DOM ke saath SPA Navigation
- ✅ Responsive Design
- ✅ Error Handling Middleware
- ✅ CORS Configuration
- ✅ Environment Variables Support

---

## 📸 Screenshots

> Yahan apne project ke screenshots add karein

| Page        | Preview |
|-------------|---------|
| Home Page   | ![Home](#) |
| Login Page  | ![Login](#) |
| Dashboard   | ![Dashboard](#) |

---

## 🤝 Contributing

Contributions welcome hain! Agar aap contribute karna chahte hain:

1. Repository ko **Fork** karein
2. Apni feature branch banayein: `git checkout -b feature/amazing-feature`
3. Changes commit karein: `git commit -m 'Add amazing feature'`
4. Branch push karein: `git push origin feature/amazing-feature`
5. **Pull Request** open karein

---

## 📄 License

Yeh project [MIT License](LICENSE) ke under licensed hai.

---

## 👨‍💻 Author

**Your Name**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: [your-linkedin](https://linkedin.com/in/your-linkedin)
- Email: your.email@example.com

---

<div align="center">
  ⭐ Agar yeh project helpful laga toh <strong>Star</strong> zaroor dein!
</div>
