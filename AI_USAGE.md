# BÁO CÁO SỬ DỤNG AI (AI_USAGE.md)

## 1. Công cụ AI sử dụng
- ChatGPT / Gemini.

## 2. Các Prompt tiêu biểu đã sử dụng

### Prompt 1: Phân tích và rà soát HTML
> "Tôi đang làm bài tập cá nhân môn Phát triển ứng dụng TMĐT Buổi 2. Đây là mã HTML từ Buổi 1. Hãy giúp tôi phân tích 3 vấn đề về bố cục và đề xuất cách cải thiện bằng HTML5 semantic và CSS3."

### Prompt 2: Hướng dẫn Flexbox & Grid
> "Tôi muốn sử dụng CSS Grid cho danh sách 4 sản phẩm và Flexbox cho thanh header. Hãy hướng dẫn tôi thiết lập grid-template-columns, gap và object-fit: cover để hình ảnh không bị méo."

### Prompt 3: Kiểm tra Lỗi và Responsive
> "Hãy kiểm tra xem đoạn mã media query của tôi đã phù hợp cho kích thước điện thoại (390px) chưa và hướng dẫn tôi bổ sung hiệu ứng hover/focus mượt mà."

## 3. Đánh giá và Tự điều chỉnh kết quả của AI
- AI gợi ý mã CSS Grid ban đầu chưa có thuộc tính `minmax(0, 1fr)`, em đã tự bổ sung vào `.product-grid` để tránh bị nổ khung (overflow) trên màn hình nhỏ.
- Em đã trực tiếp test và xác nhận hình ảnh hiển thị đúng tỷ lệ, nút bấm tương tác mượt và mã nguồn tuân thủ đúng yêu cầu của tài liệu Buổi 2 UEH.
