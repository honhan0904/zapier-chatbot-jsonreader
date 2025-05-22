# JSON Reader for Zapier Interface Design

![Zapier JSON Reader](https://via.placeholder.com/600x300?text=JSON+Reader+for+Zapier)  
*Một giao diện đơn giản và tối ưu hóa để đọc, lọc và xử lý JSON cho chatbot Zapier.*

## Giới thiệu
Đây là tài liệu mô tả thiết kế giao diện cho một website chuyên dụng để đọc và quản lý dữ liệu JSON, chỉ dành cho Zapier chatbot. Website này bao gồm các tính năng như kiểm tra/merge dữ liệu, lọc theo ngày/giờ/phút, chọn tất cả, highlight tìm kiếm, checkbox độc lập, đếm số đối thoại (với cảnh báo spam), và tối ưu hóa giao diện cho dễ nhìn.

Nếu bạn đang phát triển một dự án liên quan, tài liệu này có thể dùng làm hướng dẫn để xây dựng hoặc cải tiến giao diện.

## Tính năng chính
Dựa trên yêu cầu, giao diện sẽ hỗ trợ các tính năng sau:
- **Kiểm tra và merge dữ liệu JSON**: Cho phép người dùng kiểm tra và kết hợp dữ liệu từ nhiều file JSON.
- **Lọc theo ngày, giờ, phút**: Thêm bộ lọc thời gian để dễ dàng lọc dữ liệu.
- **Chọn tất cả (Select All)**: Tùy chọn chọn toàn bộ dữ liệu, kể cả trong phần lọc.
- **Highlight giá trị tìm kiếm**: Tô màu vàng cho các giá trị khớp với tìm kiếm.
- **Checkbox độc lập**: Không sử dụng dropdown; mỗi checkbox hoạt động riêng lẻ.
- **Đếm số đối thoại**: Tính số lượng đối thoại trong một ConversationID (ví dụ: nếu >3, đánh dấu là spam).
- **Tối ưu hóa đọc**: Làm cho giao diện dễ đọc hơn với màu sắc, font chữ và bố cục rõ ràng.

## Thiết kế giao diện đề xuất
Dưới đây là mô tả chi tiết về cách thiết kế giao diện để làm cho nó "đẹp" và dễ sử dụng. Tôi sử dụng nguyên tắc UI/UX tối giản, responsive và hấp dẫn.

### Cấu trúc tổng thể
- **Header**: Phần đầu trang với logo, tiêu đề và thanh tìm kiếm.
- **Main Content**: Khu vực chính để hiển thị dữ liệu JSON, bộ lọc và tương tác.
- **Sidebar/Footer**: Phần phụ cho tùy chọn nhanh và thông tin bổ sung.

#### 1. Header
- Hiển thị tiêu đề **"JSON Reader for Zapier"** với font lớn, màu xanh dương (#007BFF).
- Thanh tìm kiếm: Ô input với placeholder "Tìm kiếm giá trị JSON...".
- Nút "Select All": Icon checkbox, khi click sẽ chọn tất cả dữ liệu.

#### 2. Main Content
- **Bộ lọc**: 
  - Lọc theo ngày/giờ/phút: Sử dụng input date-time (ví dụ: sử dụng thư viện như Flatpickr).
  - Checkbox "Chọn tất cả trong bộ lọc".
- **Hiển thị dữ liệu JSON**:
  - Sử dụng bảng hoặc cây JSON để hiển thị.
  - Mỗi hàng có checkbox độc lập.
  - Đếm đối thoại: Hiển thị badge như "Số đối thoại: 5 (Spam?)" với màu đỏ nếu >3.
  - Highlight: Giá trị tìm kiếm được tô màu vàng (#FFD700).
- Nút "Merge Selected": Để kết hợp dữ liệu đã chọn.

#### 3. Sidebar
- Các nút nhanh: "Load JSON File", "Export Merged Data".
