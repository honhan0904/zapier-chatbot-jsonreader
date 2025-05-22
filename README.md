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
