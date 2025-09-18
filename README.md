# Real-Time Employee Task Management Tool 🚀

Một hệ thống quản lý nhân sự **real-time** bao gồm:
- 👨‍💼 Quản lý nhân viên
- ✅ Quản lý công việc
- 🔑 Đăng nhập/Đăng ký + phân quyền
- 💬 Chat real-time (Socket.io)
- 📊 Dashboard quản lý trực quan  

Dự án được xây dựng với **Node.js (Express + Socket.io + PostgreSQL)** cho backend và **React + Vite** cho frontend.

---

## 📂 Cấu trúc thư mục

```bash
project-root/
│── backend/                      # Backend (Node.js + Express + PostgreSQL)
│   ├── src/
│   │   ├── config/               # Cấu hình (DB, env, etc.)
│   │   ├── models/               # ORM/Models (Employee, User,...)
│   │   ├── controllers/          # Xử lý request
│   │   ├── services/             # Business logic
│   │   ├── routes/               # API endpoints
│   │   ├── utils/                # Tiện ích (JWT, hash password,...)
│   │   ├── app.js                # Express config
│   │   └── server.js             # Chạy server + socket.io
│   ├── package.json
│   └── .env                      # Env: DB_URL, JWT_SECRET,...
│
│── frontend/                     # Frontend (React + Vite)
│   ├── src/
│   │   ├── assets/               # Hình ảnh, icon
│   │   ├── components/           # Components tái sử dụng
│   │   ├── pages/                # Các trang (Login, Dashboard,...)
│   │   ├── services/             # Gọi API backend
│   │   ├── context/              # Context API (Auth, Socket,...)
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── vite.config.js
│   ├── package.json
│   └── .env                      # Env: VITE_API_URL,...
│
│── docker-compose.yml             # Chạy backend + db bằng Docker (tuỳ chọn)
│── README.md
⚙️ Công nghệ sử dụng
Backend:
Node.js
Express.js
PostgreSQL
[Sequelize hoặc Knex] (tùy bạn chọn ORM)
JWT
 cho xác thực
Socket.io
 cho chat real-time
Frontend:
React
 + Vite
TailwindCSS
 để styling
Axios
 để gọi API
[Context API] quản lý state (Auth, Socket)
🚀 Cách chạy dự án
1. Clone repo
git clone https://github.com/<your-username>/Real-Time-Employee-Task-Management-Tool.git
cd Real-Time-Employee-Task-Management-Tool

2. Cài dependencies
Backend
cd backend
npm install

Frontend
cd frontend
npm install

3. Tạo file .env
Backend (backend/.env)
PORT=5000
DB_URL=postgresql://user:password@localhost:5432/employee_db
JWT_SECRET=your_jwt_secret

Frontend (frontend/.env)
VITE_API_URL=http://localhost:5000

4. Chạy ứng dụng
Backend
cd backend
npm run dev

Frontend
cd frontend
npm run dev


Mở trình duyệt tại:
👉 Frontend: http://localhost:5173
👉 Backend API: http://localhost:5000

🐳 Chạy với Docker (tuỳ chọn)
docker-compose up --build

📌 Tính năng chính

🔑 Đăng nhập/Đăng ký (JWT Authentication)

👨‍💼 Quản lý nhân viên (CRUD)

📋 Quản lý công việc

📊 Dashboard trực quan

💬 Chat real-time giữa nhân viên & quản lý

⚡ Đồng bộ dữ liệu real-time với Socket.io

✨ Hướng phát triển

Gửi thông báo (Notification real-time)

Phân quyền nâng cao (Admin/Manager/Employee)

Tích hợp CI/CD (GitHub Actions)

Deploy lên Vercel (FE) + Render/Heroku (BE)
<img width="1613" height="1168" alt="image" src="https://github.com/user-attachments/assets/47e5e917-0d79-4c9f-887f-1cc4f8a3afb3" />

👨‍💻 Tác giả

Quang Nhật Phi Yến 🚀
📧 Liên hệ: [your-email@example.com
]
🌐 GitHub: https://github.com/quangnhatphiyen
