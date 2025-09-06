# OnThiUI - Hệ thống E-Learning

## Mô tả dự án

OnThiUI là một ứng dụng web E-Learning được xây dựng bằng Angular, cung cấp nền tảng học tập trực tuyến với các tính năng:

- **Quản lý khóa học**: Tạo, chỉnh sửa và quản lý khóa học
- **Hệ thống người dùng**: Phân quyền Admin, Teacher, Student
- **Chat real-time**: Tính năng chat với WebSocket
- **Quản lý bài học**: Upload video, tài liệu, bài tập
- **Lịch học**: Quản lý lịch trình học tập
- **Thanh toán**: Tích hợp mua khóa học

## Công nghệ sử dụng

- **Frontend**: Angular 15+
- **Styling**: Less CSS
- **Real-time**: WebSocket (RxStomp)
- **UI Components**: Custom components
- **File Upload**: Tích hợp upload file/video
- **Authentication**: JWT Token

## Cài đặt và chạy dự án

### Yêu cầu hệ thống
- Node.js (v16+)
- npm hoặc yarn
- Angular CLI

### Các bước cài đặt

1. **Clone repository**
```bash
git clone https://github.com/YOUR_USERNAME/OnThiUI.git
cd OnThiUI
```

2. **Cài đặt dependencies**
```bash
npm install
```

3. **Cài đặt các package bổ sung**
```bash
npm install --save --force tinymce @tinymce/tinymce-angular
npm i ngx-doc-viewer@1.4.1
```

4. **Chạy ứng dụng**
```bash
ng serve
```

5. **Truy cập ứng dụng**
Mở trình duyệt và truy cập: `http://localhost:4200`

## 📁 Cấu trúc dự án

```
src/
├── app/
│   ├── authentication/     # Module xác thực
│   ├── pages/             # Các trang chính
│   │   ├── admin/         # Trang admin
│   │   ├── teacher/       # Trang giáo viên
│   │   └── user/          # Trang học viên
│   ├── service/           # Các service
│   ├── shared/            # Components dùng chung
│   └── models/            # Data models
├── assets/                # Tài nguyên tĩnh
└── environments/          # Cấu hình môi trường
```

## 👥 Phân quyền người dùng

- **Admin**: Quản lý toàn bộ hệ thống, duyệt khóa học
- **Teacher**: Tạo và quản lý khóa học, quản lý học viên
- **Student**: Tham gia khóa học, làm bài tập, chat

## 🔧 Tính năng chính

### Cho Admin
- Quản lý người dùng
- Duyệt khóa học
- Quản lý yêu cầu khóa học

### Cho Teacher
- Tạo và chỉnh sửa khóa học
- Upload video và tài liệu
- Quản lý học viên
- Tạo bài tập và kiểm tra

### Cho Student
- Đăng ký và tham gia khóa học
- Xem video bài học
- Làm bài tập
- Chat với giáo viên
- Quản lý lịch học

## 📱 Responsive Design

Ứng dụng được thiết kế responsive, hỗ trợ tốt trên:
- Desktop
- Tablet
- Mobile

## 🔐 Bảo mật

- JWT Authentication
- Route Guards
- HTTP Interceptors
- Input validation

## 📞 Liên hệ

Nếu có thắc mắc về dự án, vui lòng liên hệ qua GitHub Issues.

---

**Lưu ý**: Dự án này được phát triển cho mục đích học tập và phỏng vấn.