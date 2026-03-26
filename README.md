# 🏡 WanderLust (Airbnb Clone)

> 🌍 Explore the World, One Booking at a Time

---

## 🚀 Highlights
- Built a full-stack CRUD application with real-world architecture  
- Designed RESTful APIs using Express  
- Implemented server-side rendering using EJS  
- Structured project following MVC principles (in progress)

---

## 📋 Description

WanderLust is a dynamic web application that allows users to browse, create, and manage property listings. Unlike traditional MERN SPAs, this project uses **server-side rendering (EJS)** for faster development and simplified architecture.

This project is being built incrementally to simulate a **real-world production workflow**.

---

## 🎯 Why This Project?

This project was built to:
- Understand backend system design  
- Implement RESTful APIs  
- Build a scalable MVC-based application  
- Simulate real-world product development  

---

## ✨ Key Features

- 🏠 Full CRUD operations for property listings  
- 📦 Database seeding with mock data  
- 🎨 Dynamic UI using EJS templating (`ejs-mate`)  
- 📱 Responsive design with Bootstrap 5  
- 🔁 RESTful routing with method-override  

---

## 🚧 Current Status

**⚠️ Early Development Phase**

- Backend CRUD operations are fully functional  
- MongoDB integration is complete  
- EJS-based UI structure is set up  
- Core architecture is established  

**🚧 Currently working on:**
- Authentication system  
- Image upload (Cloudinary + Multer / ImageKit)  
- Error handling & validation  

---

## 🏗️ Architecture Overview

```text
Client (Browser)
       ↓
Express Server (app.js)
       ↓
Routes & Controllers
       ↓
Mongoose Models
       ↓
MongoDB Database
```

## 📂 Project Structure

```text
airbnb-clone/
├── app.js
├── package.json
├── init/
│   ├── index.js
│   └── data.js
├── models/
│   └── listing.js
├── public/
│   └── css/
│       └── style.css
└── views/
    ├── includes/
    ├── layouts/
    └── listings/
```

## 🛠️ Tech Stack
- **Backend:** Node.js, Express.js
- **Database:** MongoDB + Mongoose
- **Frontend:** EJS (Server-Side Rendering), Bootstrap 5
- **Templating Engine:** ejs-mate
- **Other Tools:** method-override, dotenv (planned)

## 📡 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| GET | `/` | Server check |
| GET | `/listings` | Get all listings |
| GET | `/listings/new` | Create listing form |
| POST | `/listings` | Add new listing |
| GET | `/listings/:id` | View single listing |
| GET | `/listings/:id/edit` | Edit form |
| PUT | `/listings/:id` | Update listing |
| DELETE | `/listings/:id` | Delete listing |

## ⚙️ Installation & Setup

### Prerequisites
- Node.js
- MongoDB (running locally)

### Setup

```bash
# Clone repo
git clone <your-repo-url>
cd airbnb-clone

# Install dependencies
npm install

# Seed database
node init/index.js

# Run server
node app.js
```

Server runs on:
👉 `http://localhost:5050`

## 🔐 Environment Variables

Create a `.env` file:

```env
PORT=5050
MONGO_URL=mongodb://127.0.0.1:27017/wanderlust

# Future use
IMAGEKIT_PUBLIC_KEY=your_public_key
IMAGEKIT_PRIVATE_KEY=your_private_key
IMAGEKIT_URL_ENDPOINT=https://your-url-endpoint

# Security
SESSION_SECRET=your_secure_secret
```

## ⚠️ Current Limitations
- No authentication (anyone can modify listings)
- No authorization checks
- No server-side validation
- No centralized error handling
- No testing framework

## 🚀 Future Improvements

🎯 Goal: Transform this into a production-ready Airbnb-like platform

### 🔥 Must Have
- User authentication (Passport.js / JWT)
- Authorization (owner-based access control)
- MVC restructuring (separate routes/controllers)
- Error handling middleware

### 👍 Good to Have
- Image upload with Cloudinary / ImageKit
- Form validation (Joi)
- Reviews & ratings system
- Map integration (Mapbox)

### 🚀 Advanced
- Booking & reservation system
- Payment integration (Stripe)
- Convert to full MERN (React frontend)
- Deployment (AWS / Docker)

## 🧠 Developer Insights
- Follows basic MVC pattern but needs modularization
- `app.js` is currently overloaded (needs refactoring)
- Lacks async error handling (risk of crashes)
- Strong foundation for scaling into a production-grade app

## 🤝 Contributing

Contributions are welcome!

```bash
git checkout -b feature/YourFeature
git commit -m "Add feature"
git push origin feature/YourFeature
```

## 📄 License

Licensed under ISC License.

## 👤 Author

**Valurothu Sharan**

## ⭐ Support

If you like this project:

⭐ Give it a star on GitHub  
💬 Share feedback  
🚀 Suggest improvements  