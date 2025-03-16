# 📊 MOOLI-BI

A free, open-source **Business Intelligence Tool** designed for small businesses in India. This tool allows users to upload datasets, generate interactive visualizations, and gain valuable insights from their data.

---

## 🚀 Features
- **User Authentication**: Secure login & signup with JWT authentication.
- **Data Upload**: Upload Excel files for analysis.
- **Data Visualization**: Generate dynamic charts & reports.
- **Decentralized File Storage**: Supports blockchain-based storage for security.
- **Role-Based Access**: Different permissions for admin & users.

---

## 🏗 Tech Stack
### **Frontend (React.js)**
- React with Vite
- Tailwind CSS
- React Router
- Axios
- Recharts (for data visualization)

### **Backend (Node.js & Express.js)**
- Express.js (REST API)
- MongoDB (Mongoose ORM)
- JWT Authentication
- CORS Handling
- Multer (for file uploads)

### **Deployment**
- **Frontend**: Vercel
- **Backend**: Vercel
- **Database**: MongoDB Atlas

---

## 📦 Installation & Setup
### 1️⃣ **Clone the Repository**
```sh
git clone git@github.com:Prayrit9/MOOLI-BI.git
cd MOOLI-BI
```

### 2️⃣ **Backend Setup**
```sh
cd backend
npm install
```
Create a `.env` file and add:
```env
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
```
Run the server:
```sh
npm start
```

### 3️⃣ **Frontend Setup**
```sh
cd ../frontend
npm install
```
Update `api.js` with your backend URL:
```js
const API_BASE_URL = "https://your-backend-url.vercel.app/api";
```
Run the frontend:
```sh
npm run dev
```

---

## 🌍 Deployment (Vercel)
### **Deploy Backend**
```sh
cd backend
vercel
```

### **Deploy Frontend**
```sh
cd frontend
vercel
```

---


---

## ❓ Troubleshooting
### **CORS Issues**
If you face CORS errors, ensure the backend has this middleware:
```js
const cors = require("cors");
app.use(cors({ origin: "https://your-frontend-url.vercel.app" }));
```

### **Common Errors & Fixes**
| Error | Solution |
|-------|----------|
| `CORS policy error` | Add `Access-Control-Allow-Origin` in backend |
| `MongoDB connection failed` | Check `.env` for correct MongoDB URI |
| `Deployment failed on Vercel` | Run `vercel env add VARIABLE_NAME` |

---

## 🤝 Contributing
1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit changes: `git commit -m "Add new feature"`
4. Push to GitHub: `git push origin feature-name`
5. Open a Pull Request

---

## 📜 License
This project is **MIT Licensed**. Feel free to use and contribute!

---

## 💡 Contact
📧 Email: [your-email@example.com](mailto:your-email@example.com)  
🐙 GitHub: [your-username](https://github.com/your-username)

---

⭐ **If you like this project, give it a star!** ⭐
