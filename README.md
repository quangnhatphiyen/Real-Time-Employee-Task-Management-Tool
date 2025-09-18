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
## ⚙️ Công nghệ sử dụng

### 🔹 Backend
- **Node.js** – Nền tảng chạy JavaScript phía server.
- **Express.js** – Framework xây dựng API nhanh gọn.
- **PostgreSQL** – Hệ quản trị cơ sở dữ liệu quan hệ.
- **Sequelize hoặc Knex** – ORM/Query builder để thao tác DB (bạn chọn 1).
- **JWT (JSON Web Token)** – Xác thực & phân quyền.
- **Socket.io** – Giao tiếp **real-time** (chat, thông báo, cập nhật dữ liệu).

### 🔹 Frontend
- **React + Vite** – Xây dựng giao diện người dùng nhanh và tối ưu.
- **TailwindCSS** – Thư viện CSS utility-first để styling.
- **Axios** – Gọi API từ frontend tới backend.
- **Context API** – Quản lý state toàn cục (Auth, User, Socket).
