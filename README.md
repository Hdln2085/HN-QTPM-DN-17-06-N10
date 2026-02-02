
<h2 align="center">
    <a href="https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin">
    🎓 Faculty of Information Technology (DaiNam University)
    </a>
</h2>
</h2>
<h2 align="center">
    PLATFORM ERP
</h2>
<div align="center">
    <p align="center">
        <img src="docs/logo/aiotlab_logo.png" alt="AIoTLab Logo" width="170"/>
        <img src="docs/logo/fitdnu_logo.png" alt="AIoTLab Logo" width="180"/>
        <img src="docs/logo/dnu_logo.png" alt="DaiNam University Logo" width="200"/>
    </p>

[![AIoTLab](https://img.shields.io/badge/AIoTLab-green?style=for-the-badge)](https://www.facebook.com/DNUAIoTLab)
[![Faculty of Information Technology](https://img.shields.io/badge/Faculty%20of%20Information%20Technology-blue?style=for-the-badge)](https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin)
[![DaiNam University](https://img.shields.io/badge/DaiNam%20University-orange?style=for-the-badge)](https://dainam.edu.vn)

</div>

## 📖 1. Giới thiệu
Platform ERP được áp dụng vào học phần Thực tập doanh nghiệp dựa trên mã nguồn mở Odoo. 

## 🔧 2. Các công nghệ được sử dụng
<div align="center">

### Hệ điều hành
[![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)](https://ubuntu.com/)
### Công nghệ chính
[![Odoo](https://img.shields.io/badge/Odoo-714B67?style=for-the-badge&logo=odoo&logoColor=white)](https://www.odoo.com/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![XML](https://img.shields.io/badge/XML-FF6600?style=for-the-badge&logo=codeforces&logoColor=white)](https://www.w3.org/XML/)
### Cơ sở dữ liệu
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
</div>

## Poster
<img width="625" height="799" alt="image" src="https://github.com/user-attachments/assets/f9803ac4-fc2e-4757-9337-c555a27f1e40" />

## 🚀 3. Hình ảnh các chức năng
![duan](https://github.com/user-attachments/assets/85f8a5ce-dc45-47b4-867c-7928334707a1)

### Trang dashboard 
<img width="1885" height="935" alt="image" src="https://github.com/user-attachments/assets/a4da6d0d-95fa-4d44-b451-519e238776a1" />
### Trang Nhân viên
<img width="1886" height="940" alt="image" src="https://github.com/user-attachments/assets/ccd99c63-f3a3-474f-a479-14d474279459" />
### Trang Dự án
<img width="1890" height="932" alt="image" src="https://github.com/user-attachments/assets/349d27b5-1e2c-4cde-8bdf-df3e6346414d" />
### Trang Chuc vu
<img width="1901" height="939" alt="image" src="https://github.com/user-attachments/assets/0903ffdb-195a-4793-a57d-3362f3dcefdd" />
### Trang Cong viec nhan vien
<img width="1892" height="938" alt="image" src="https://github.com/user-attachments/assets/6e8de269-7d69-4315-92bc-9134998ba666" />

## ⚙️ 4. Cài đặt

### 4.1. Cài đặt công cụ, môi trường và các thư viện cần thiết

- Tải và cài đặt **XAMPP**  
  👉 https://www.apachefriends.org/download.html  
  (Khuyến nghị bản XAMPP với PHP 8.x)

- Cài đặt **Visual Studio Code** và các extension:
  - PHP Intelephense  
  - MySQL  
  - Prettier – Code Formatter  
### 4.2. Tải project
Clone project về thư mục `htdocs` của XAMPP (ví dụ ổ C):

```bash
cd C:\xampp\htdocs
https://github.com/dk123-bb/TTDN-16-05-N7/tree/main/addons
Truy cập project qua đường dẫn:
👉 https://github.com/dk123-bb/TTDN-16-05-N7
```
### 4.3. Setup database
Mở XAMPP Control Panel, Start Apache và MySQL

Truy cập MySQL WorkBench
Tạo database:
```bash
CREATE DATABASE IF NOT EXISTS quan_ly_doan_vien
   CHARACTER SET utf8mb4
   COLLATE utf8mb4_unicode_ci;
```

### 4.4. Setup tham số kết nối
Mở file config.php (hoặc .env) trong project, chỉnh thông tin DB:
```bash

<?php
    function getDbConnection() {
        $servername = "localhost";
        $username = "root";
        $password = "";
        $dbname = "quan_ly_cong_viec;
        $port = 3306;
        $conn = mysqli_connect($servername, $username, $password, $dbname, $port);
        if (!$conn) {
            die("Kết nối database thất bại: " . mysqli_connect_error());
        }
        mysqli_set_charset($conn, "utf8");
        return $conn;
    }
?>
```
### 4.5. Chạy hệ thống
Mở XAMPP Control Panel → Start Apache và MySQL

Truy cập hệ thống:
👉 http://localhost/index.php

### 4.6. Đăng nhập lần đầu
Hệ thống có thể cấp tài khoản admin 

Sau khi đăng nhập Admin có thể:

Tạo thông tin tổ chức đoàn (Đoàn trường, Liên chi, Chi đoàn)

Thêm đoàn viên và cấp tài khoản

Quản lý phân quyền theo cấp
---

    
