# WEB-KEY-SELLERS - Digital Asset E-commerce with AI Integration 🛒🤖

Xây dựng Website kinh doanh tài sản số tích hợp Hệ thống AI gợi ý sản phẩm & Chatbot tư vấn thông minh.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Frontend](https://img.shields.io/badge/Frontend-React%20%7C%20Vite%20%7C%20Tailwind-61DAFB)
![Backend](https://img.shields.io/badge/Backend-NestJS%20%7C%20Prisma%20%7C%20MySQL-E0234E)
![AI System](https://img.shields.io/badge/AI-Python%20%7C%20Gemini%20%7C%20RAG-FFD43B)




## 📖 Giới Thiệu Dự Án (Project Overview)

**WEB-KEY-SELLERS** (WEBKey) không chỉ là một website bán hàng thông thường mà là giải pháp công nghệ tập trung giải quyết các vấn đề cốt lõi trong giao dịch tài sản số (Digital Assets) như: Key bản quyền, Tài khoản Premium (Netflix, Spotify, Youtube...), Phần mềm, Game.

Hệ thống tích hợp **Trợ lý ảo Fairy** sử dụng công nghệ RAG (Retrieval-Augmented Generation) giúp tư vấn chính xác theo thời gian thực và Hệ thống gợi ý sản phẩm cá nhân hóa (Recommendation System).

## 🚀 Tính Năng Đột Phá (Key Features)

Dự án tập trung giải quyết 3 bài toán kỹ thuật cốt lõi:

### 1. An Toàn Tài Chính (Financial Security) 🛡️
* **Cơ chế:** Xác thực hai bước (Admin Approval).
* **Mô tả:** Mọi giao dịch xuất kho Key đều yêu cầu Admin phê duyệt sau khi đối soát mã giao dịch ngân hàng, loại bỏ triệt để rủi ro gian lận thanh toán (Fake Bill).

### 2. Khóa Giao Dịch (Concurrency Control) 🔒
* **Cơ chế:** Stock Reservation (Giữ chỗ thông minh).
* **Mô tả:** Ngay khi User đặt đơn, hệ thống lập tức khóa Key ở trạng thái `Pending/Reserved`. Giải quyết triệt để vấn đề **Race Condition** (nhiều người cùng mua 1 sản phẩm tại cùng 1 thời điểm).

### 3. Trí Tuệ Nhân Tạo Thế Hệ Mới (Next-Gen AI) 🧠
* **Chatbot RAG (Fairy):**
    * Tích hợp **Google Gemini LLM** với cơ sở dữ liệu Vector (**ChromaDB**).
    * Khả năng tra cứu ngữ nghĩa từ tài liệu chính sách của cửa hàng (File `.md`) để trả lời chính xác, tránh hiện tượng "ảo giác" (Hallucination) của AI.
* **Hệ thống Gợi ý (Recommendation Engine):**
    * Sử dụng thuật toán **Collaborative Filtering** (Lọc cộng tác).
    * Phân tích ma trận tương tác người dùng để đề xuất sản phẩm chéo (Cross-sell) phù hợp với hành vi mua sắm (Ví dụ: Mua Youtube -> Gợi ý Netflix).

---

## 🛠️ Công Nghệ Sử Dụng (Tech Stack)

### Frontend (Giao diện người dùng)
* **ReactJS**: Library xây dựng UI/UX tương tác cao.
* **Vite**: Build tool thế hệ mới, tối ưu tốc độ phản hồi.
* **Tailwind CSS**: Framework CSS utility-first giúp xây dựng giao diện nhanh chóng.

### Backend (Hệ thống xử lý)
* **NestJS**: Framework Node.js kiến trúc module, dễ mở rộng và bảo trì.
* **MySQL**: Cơ sở dữ liệu quan hệ, đảm bảo tính toàn vẹn giao dịch.
* **Prisma ORM**: Trừu tượng hóa thao tác cơ sở dữ liệu.
* **JWT (JSON Web Token)**: Cơ chế xác thực bảo mật (Stateless Authentication).
* **Cloudinary**: Lưu trữ và tối ưu hóa hình ảnh sản phẩm.
* **VietQR**: Tích hợp thanh toán QR Code tự động.

### AI System (Hệ thống thông minh)
* **Ngôn ngữ:** Python.
* **Model:** Google Gemini API.
* **Vector DB:** ChromaDB (Lưu trữ vector kiến thức doanh nghiệp).
* **Technique:** RAG (Retrieval-Augmented Generation) & Collaborative Filtering.

### Tools & DevOps
* **IDE:** Visual Studio Code.
* **Testing:** Postman.
* **Version Control:** Git.

---

## 📂 Cấu Trúc Dự Án
```bash 
WEB-KEY-SELLERS/
├── AI_SYSTEM/          # Mã nguồn Python cho Chatbot & Recommendation
├── frontend/           # Mã nguồn ReactJS (Client & Admin Dashboard)
├── prisma/             # Schema Database & Migrations
├── src/                # Mã nguồn Backend NestJS
├── test/               # E2E Testing
└── ...
