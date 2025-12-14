# 🎥 PhimVietHay - Nền tảng Xem Phim Trực Tuyến Hiện Đại

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![React](https://img.shields.io/badge/Frontend-React_Vite-61DAFB?logo=react)
![Node](https://img.shields.io/badge/Backend-Node.js_Express-339933?logo=nodedotjs)
![Database](https://img.shields.io/badge/Database-TiDB_%2F_MySQL-4479A1?logo=mysql)
![Style](https://img.shields.io/badge/Style-Tailwind_CSS-38B2AC?logo=tailwindcss)

**PhimVietHay** là một ứng dụng web xem phim trực tuyến trọn gói (Full-stack) được xây dựng với MERN Stack (sử dụng TiDB làm cơ sở dữ liệu).  
Dự án tập trung vào trải nghiệm người dùng mượt mà, giao diện Dark Mode hiện đại và tốc độ tải trang nhanh.

---

## 🌟 Tính Năng Nổi Bật

### 👤 Xác Thực & Người Dùng
- Đăng nhập / Đăng ký bảo mật với **JWT (JSON Web Token)**  
- Đăng nhập nhanh bằng **Google OAuth**  
- **Auto Merge Account**: Tự động đồng bộ tài khoản nếu email trùng khớp  
- Quản lý hồ sơ cá nhân, cập nhật **Avatar**  

### 🎬 Trải Nghiệm Xem Phim
- Kho phim đa dạng: Phim Lẻ, Phim Bộ, TV Shows, Hoạt Hình  
- Tìm kiếm thông minh với **Debounce** (giảm tải server)  
- Bộ lọc theo **Quốc gia – Thể loại – Năm phát hành**  
- Trình phát video mượt mà, hỗ trợ **server dự phòng**  

### ❤️ Cá Nhân Hóa
- Lưu phim **Yêu thích / Xem sau**  
- Lưu **lịch sử xem & tiến độ phim**  
- Bình luận, thảo luận và đánh giá phim (**Real-time**)  

### 🛠️ Tính Năng Khác
- Responsive hoàn toàn trên **Mobile – Tablet – Desktop**  
- **Watch Party (Rạp phim online)** – đang phát triển  
- **Admin Dashboard**: Quản lý phim, người dùng, thống kê  

---

## 🚀 Công Nghệ Sử Dụng

| Phần | Công Nghệ | Chi Tiết |
| :--- | :--- | :--- |
| **Frontend** | React (Vite) | Build nhanh, SPA |
| | Tailwind CSS | UI, Responsive, Animation |
| | React Router DOM | Điều hướng |
| | Axios | HTTP Request |
| **Backend** | Node.js / Express | REST API |
| | Passport.js | Google OAuth |
| | JWT | Authentication |
| **Database** | TiDB Cloud | MySQL Compatible |
| **Deploy** | Render / Vercel | Server & Client |

---

## 🔧 Hướng Dẫn Cài Đặt (Localhost)

### 1️⃣ Clone dự án
```bash
git clone https://github.com/bebokaka99/phimviethay_git
cd phimviethay
```

### 2️⃣ Cấu hình Backend (Server)
```bash
cd server
npm install
```

Tạo file `.env` trong thư mục `server/`:
```env
PORT=5000

# Database (TiDB / MySQL)
DB_HOST=your_tidb_host
DB_PORT=4000
DB_USER=your_db_user
DB_PASS=your_db_pass
DB_NAME=test

# Security
JWT_SECRET=ma_bi_mat_jwt
ACCESS_TOKEN_SECRET=ma_bi_mat_access
REFRESH_TOKEN_SECRET=ma_bi_mat_refresh

# Client URL
CLIENT_URL=http://localhost:5173

# Google OAuth
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GOOGLE_CALLBACK_URL=http://localhost:5000/api/auth/google/callback
```

Chạy server:
```bash
npm run dev
```

### 3️⃣ Cấu hình Frontend (Client)
```bash
cd client
npm install
```

Tạo file `.env` trong `client/`:
```env
VITE_API_URL=http://localhost:5000
```

Chạy client:
```bash
npm run dev
```

👉 Truy cập: **http://localhost:5173** 🍿

---

## 🤝 Đóng Góp (Contributing)

1. Fork dự án  
2. Tạo branch mới: `git checkout -b feature/TinhNangMoi`  
3. Commit: `git commit -m "Thêm tính năng X"`  
4. Push: `git push origin feature/TinhNangMoi`  
5. Tạo Pull Request  

---

## 📄 Bản Quyền
Dự án được phát triển cho mục đích **học tập & phi lợi nhuận**.

---
