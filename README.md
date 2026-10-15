# Ứng dụng Quản lý Lịch Học Cá nhân

Ứng dụng giúp sinh viên ***lên kế hoạch học tập*** hiệu quả.

## Hướng dẫn Cài đặt

```bash
git clone [https://github.com/nhom5/lich-hoc-app](https://github.com/nhom5/lich-hoc-app)
cd lich-hoc-app
``` 
Tính năng đã hoàn thành  
[x] Đăng ký / Đăng nhập tài khoản
[ ] Nhắc nhở lịch học qua email   
[x] Xuất lịch ra file PDF   


---

Bảng So sánh Công nghệ   
| Công nghệ | PythonBackend | Markdown |
| --- | --- | --- |
| Mục đích | Backend xử lý dữ liệu | Viết tài liệu | 
| Phiên bản | 3.11 | ___ |  

---

#### **3. Bẫy dữ liệu: Nếu hàng phân cách bảng (dòng `| --- | --- | --- |`) bị xóa, bảng sẽ hiển thị như thế nào? Tại sao?**

* **Hiển thị thực tế:** Nếu hàng phân cách bảng bị xóa, trình biên dịch Markdown sẽ không nhận diện được đó là một cấu trúc bảng dữ liệu. Toàn bộ nội dung của bảng sẽ bị biến đổi thành một **đoạn văn bản thô (Plain Text)** hoặc một danh sách các dòng chữ dính liền nhau ngăn cách bởi dấu gạch đứng (`|`), hoàn toàn mất đi định dạng khung lưới, đường viền và căn chỉnh cột.
* **Nguyên nhân:** Bộ phân tích cú pháp Markdown quy định dòng phân cách (chứa dấu `-` kết hợp với dấu `|`) chính là "chìa khóa" cốt lõi để xác định phần trên là hàng tiêu đề (Header row) và các dòng dưới là dữ liệu nội dung của bảng. Thiếu dòng này, thuật toán xử lý mất đi mốc nhận diện cấu trúc bảng.
