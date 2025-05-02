
# Ứng dụng phương thức kiểm thử thủ công và kiểm thử tự động cho website Bán thực phẩm

## 🎓 Báo cáo khóa luận tốt nghiệp

Đây là dự án phục vụ cho báo cáo khóa luận tốt nghiệp với đề tài **"Ứng dụng phương thức kiểm thử thủ công và kiểm thử tự động cho website Bán thực phẩm"**. Mục tiêu chính là áp dụng và đánh giá hiệu quả của hai phương pháp kiểm thử (manual & automation) trên các chức năng quan trọng của một hệ thống đặt hàng thực phẩm trực tuyến.

## 📌 Mục tiêu

- Áp dụng kiểm thử thủ công để xác thực chức năng.
- Phát triển kịch bản kiểm thử tự động bằng Selenium WebDriver.
- So sánh hiệu quả, độ chính xác và độ bao phủ giữa hai phương pháp kiểm thử.

## 🧪 Các chức năng được kiểm thử

1. **Trang Đăng nhập**
   - Kiểm thử đăng nhập đúng/sai cho người dùng và quản trị viên.
2. **Thêm sản phẩm vào giỏ hàng**
   - Thêm sản phẩm từ danh sách vào giỏ hàng.
3. **Trang Giỏ hàng**
   - Hiển thị số lượng sản phẩm, tính tổng giá, cập nhật và xóa sản phẩm.
4. **Thông tin nhận hàng**
   - Nhập và xác thực thông tin người nhận trước khi đặt hàng.
5. **Đặt đơn hàng**
   - Gửi đơn hàng, kiểm tra phản hồi và thông báo thành công.
6. **Lịch sử đặt hàng**
   - Hiển thị các đơn hàng đã đặt và trạng thái đơn hàng trong tài khoản người dùng.

## ⚙️ Công nghệ sử dụng

- **Ngôn ngữ lập trình:** Java
- **Công cụ kiểm thử tự động:** Selenium WebDriver
- **Công cụ xây dựng:** Maven
- **Báo cáo kiểm thử:** Allure
- **Môi trường phát triển:** Eclipse
- **Nền tảng website:** PHP (chạy bằng XAMPP)

## 🔧 Hướng dẫn cài đặt website (XAMPP)

1. **Cài đặt XAMPP**:
   - Tải từ trang [https://www.apachefriends.org/](https://www.apachefriends.org/).
   - Khởi động Apache và MySQL từ XAMPP Control Panel.

2. **Cài đặt cơ sở dữ liệu**:
   - Truy cập `http://localhost/phpmyadmin`.
   - Tạo database tên `banthucpham` và import file `banthucpham.sql`.

3. **Triển khai website**:
   - Chép mã nguồn vào thư mục `htdocs`, ví dụ: `C:\xampp\htdocs\BanThucPham`.
   - Truy cập website qua đường dẫn `http://localhost/BanThucPham`.

4. **Cấu hình đường dẫn trong test code**:
   - Đảm bảo các đoạn mã test trỏ đến đúng địa chỉ `http://localhost/BanThucPham`.

## 🚀 Chạy kiểm thử tự động

1. **Clone dự án**:
   ```bash
   git clone https://github.com/HuaThao/Manual-and-Automated-Testing-WebSite-BanThucPham.git
   ```

2. **Cài đặt thư viện phụ thuộc**:
   ```bash
   mvn clean install
   ```

3. **Chạy kiểm thử**:
   ```bash
   mvn test
   ```

4. **Xem báo cáo Allure (nếu đã cấu hình)**:
   ```bash
   allure serve target/allure-results
   ```

## 📁 Cấu trúc dự án

```
├── src/
│   └── test/java/tests/
├── database/
│   └── banthucpham.sql
├── pom.xml
├── README.md
└── ...
```

## 📄 Các tài liệu đính kèm

- Tài liệu test case thủ công (Excel hoặc PDF)
- Mã nguồn kiểm thử tự động bằng Selenium
- Báo cáo khóa luận (PDF)

## 👤 Thông tin sinh viên thực hiện

- Họ tên: Hứa Văn Thảo
- MSSV: 3120221461
- Trường: Trường Đại học Sư Phạm Đà Nẵng
- Email: 3120221461@ued.udn.vn
