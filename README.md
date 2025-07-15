# Full-Stack Blog App using MERN with Secure Auth & Media Upload

This is a full-stack blogging platform developed by **Maaz Ansari**, featuring secure user authentication, media upload support, and a dynamic frontend interface. Built using the powerful MERN stack, MongoDB, Express, React, and Node.js, the project demonstrates modern web development practices including API handling, JWT-based security, image upload with Multer, and modular backend architecture.

## 🔧 Tech Stack & Why It Was Used

- **MongoDB**: A flexible NoSQL database perfect for blog content, comments, and users.
- **Express.js**: Lightweight Node.js framework used to create clean RESTful APIs and handle middleware.
- **React.js**: Enables component-based frontend development with smooth routing and dynamic rendering.
- **Node.js**: Provides an asynchronous, event-driven runtime environment to power the server.
- **Multer**: Handles media file uploads (images) via `multipart/form-data`, storing them securely.
- **JWT (JSON Web Tokens)**: Implements secure, stateless user authentication for login and route protection.
- **bcryptjs**: Used for hashing user passwords securely before storing them in the database.
- **Axios**: For smooth client-to-server API communication.

## 🔐 Features

- Register and login functionality with JWT token handling
- Password hashing and secure credential storage
- Protected routes and user sessions
- Create, edit, and delete blog posts
- Upload blog cover images using Multer
- Clean, mobile-friendly UI with responsive design

## 📁 Project Structure

```
Blog-Website/
├── client/      # React frontend (UI + routes)
├── server/      # Node + Express backend (API + DB logic)
│   ├── models/      # Mongoose schemas
│   ├── routes/      # Express routes
│   ├── controllers/ # Logic and DB calls
│   ├── middleware/  # Auth & upload middlewares
```

## 🚀 How to Run This Project in VS Code

1. **Clone the repository**
```bash
git clone https://github.com/AnsariTech-25667/Blog-Website.git
cd Blog-Website
```

2. **Install dependencies**
```bash
cd client
npm install
cd ../server
npm install
```

3. **Start the servers**
```bash
# Backend
cd server
npm run dev

# Frontend (in new terminal)
cd ../client
npm start
```

Access the app at `http://localhost:3000`.

## 🌐 Deployment Instructions

### 🔹 Deploy Backend to Render
1. Go to [https://render.com](https://render.com)
2. Click on **New Web Service**
3. Connect your GitHub repo
4. Choose `server/` as the root directory
5. Add the environment variables (`MONGO_URI`, `JWT_SECRET`, etc.)
6. Build Command: `npm install`
7. Start Command: `npm run dev`

### 🔹 Deploy Frontend to Vercel
1. Go to [https://vercel.com](https://vercel.com)
2. Click on **New Project**
3. Connect your GitHub account and select the repo
4. Choose `client/` as the project root
5. Add necessary environment variables (`REACT_APP_API_URL`, etc.)
6. Deploy

## ⚙️ GitHub Actions (CI/CD)

This project includes a sample GitHub Actions workflow `deploy.yml` (in `.github/workflows/`) to automate builds and test deployments. You can customize this for CI/CD pipelines.


