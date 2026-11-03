# BÀI TẬP CÁ NHÂN - BUỔI 2: HTML5 & CSS3
**Môn học:** Phát triển ứng dụng Web / TMĐT  
**Giảng viên hướng dẫn:** TS. Nguyễn Mạnh Tuấn - UEH  
**Dự án tiếp nối Buổi 1:** Website thương mại điện tử thời trang (Coolmate Demo / ShopMate)

---

## 1. Giới thiệu tổng quan
Bài tập thực hành củng cố cấu trúc ngữ nghĩa HTML5 và áp dụng CSS3 (Box Model, Flexbox, Grid, Responsive) để hoàn thiện khu vực trọng tâm: **Danh sách sản phẩm nổi bật & Thẻ sản phẩm (Product Card)**.

## 2. Cấu trúc thư mục dự án
Tuân thủ đúng chuẩn cấu trúc yêu cầu:
```text
my-store/
├── index.html
├── products.html
├── product-detail.html
├── about.html
├── css/
│   └── style.css
├── images/
│   ├── product-1.jpg
│   ├── product-2.jpg
│   ├── product-3.jpg
│   └── product-4.jpg
├── README.md
└── AI_USAGE.md
```

## 3. Kỹ thuật HTML5 & CSS3 đã thực hành
- **HTML5 Semantic:** Sử dụng `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`, `<img>` kèm `alt`.
- **CSS Box Model:** Thiết lập `box-sizing: border-box`, tinh chỉnh `margin`, `padding`, `border`, `border-radius`.
- **CSS Flexbox:** Căn chỉnh header, menu điều hướng, hàng hiển thị giá (`.price-row`) bằng `display: flex`, `justify-content: space-between`, `align-items: center`, `gap`.
- **CSS Grid:** Bố trí danh sách sản phẩm 4 cột trên PC, 2 cột trên Tablet/Mobile bằng `display: grid`, `grid-template-columns: repeat(4, minmax(0, 1fr))`, `gap`.
- **Hiệu ứng & Responsive:** Sử dụng `:hover`, `transition`, `:focus-visible` và `@media (max-width: 900px)`, `@media (max-width: 560px)`.

---

## 4. Trả lời 7 câu hỏi kiểm tra kiến thức (Mục 12)

### Câu 1. Trong khu vực giao diện của em, em đã sử dụng những phần tử HTML5 nào? Vì sao em chọn chúng?
- Em đã sử dụng `<header>` (đầu trang), `<nav>` (menu điều hướng), `<main>` (nội dung chính), `<section>` (khối nội dung danh sách sản phẩm), `<article>` (thẻ sản phẩm độc lập), `<h3>` (tiêu đề sản phẩm) và `<button>` (nút thao tác). Em chọn chúng vì mang tính ngữ nghĩa (semantic) rõ ràng, giúp trình duyệt và công cụ tìm kiếm dễ phân tích cấu trúc trang web.

### Câu 2. Giải thích sự khác nhau giữa margin và padding. Cho ví dụ từ thẻ sản phẩm của em.
- `padding` là khoảng cách bên trong tính từ viền khung vào nội dung. `margin` là khoảng cách bên ngoài giữa phần tử với các yếu tố xung quanh.
- *Ví dụ:* Trong `.product-card`, `padding` tạo khoảng hở giúp thông tin không bị dính sát vào viền thẻ, còn `gap`/`margin` tạo khoảng cách giữa các thẻ sản phẩm với nhau.

### Câu 3. Trong bài của em, Flexbox được sử dụng ở đâu? Giải thích tác dụng của justify-content và align-items.
- Flexbox được dùng ở thanh header (`.site-header`), hàng chứa giá (`.price-row`) và khối lợi ích (`.benefits`).
- `justify-content` giúp căn chỉnh phần tử theo chiều ngang (trục chính), ví dụ `space-between` giúp đẩy logo và menu về 2 đầu.
- `align-items` giúp căn chỉnh các phần tử theo chiều dọc (trục phụ), ví dụ `center` giúp các liên kết và logo nằm thẳng hàng giữa.

### Câu 4. CSS Grid khác Flexbox như thế nào? Vì sao em sử dụng Grid cho danh sách sản phẩm?
- Flexbox là bố cục 1 chiều (hàng hoặc cột), còn CSS Grid là bố cục 2 chiều (quản lý đồng thời cả hàng và cột).
- Em sử dụng Grid cho danh sách sản phẩm vì Grid cho phép chia cột dạng lưới (`grid-template-columns`) và tạo khoảng cách đều (`gap`) rất nhanh chóng và chuyên nghiệp cho e-commerce.

### Câu 5. Nếu xóa quy tắc CSS display: grid khỏi danh sách sản phẩm, giao diện có thể thay đổi như thế nào?
- Các thẻ sản phẩm `<article>` sẽ quay về hiển thị mặc định (dạng khối block), xếp thành 1 cột dọc kéo dài từ trên xuống dưới thay vì đứng cạnh nhau thành dàn lưới 4 cột.

### Câu 6. Vì sao cần sử dụng thuộc tính alt cho hình ảnh sản phẩm?
- Thuộc tính `alt` mô tả văn bản thay thế cho hình ảnh khi mạng bị lỗi không tải được ảnh, hỗ trợ trình đọc màn hình cho người khiếm thị và giúp tối ưu hóa tìm kiếm (SEO).

### Câu 7. Hãy nêu một đề xuất của AI mà em đã kiểm tra hoặc điều chỉnh trước khi đưa vào bài tập.
- AI đề xuất dùng `font-size: clamp(...)` cho tiêu đề `<h1>` và `<h2>`. Em đã test trên Chrome DevTools ở các độ rộng màn hình khác nhau (1366px, 768px, 390px) và nhận thấy chữ co giãn rất mượt mà nên đã áp dụng vào mã nguồn.

---

## 5. Bảng kiểm thử giao diện & Báo cáo sửa lỗi (Bước 8)

| Nội dung kiểm tra | Kết quả | Ghi chú |
| :--- | :--- | :--- |
| Trang HTML mở được | Đạt | Chạy trực tiếp file `index.html` trên trình duyệt Chrome |
| CSS được áp dụng | Đạt | Liên kết `css/style.css` chính xác, màu sắc và font chữ hiển thị đúng |
| Hình ảnh hiển thị đúng | Đạt | Hình ảnh hiển thị vuông vắn, không bị méo nhờ `object-fit: cover` |
| Liên kết hoạt động | Đạt | Các thẻ `<a>` điều hướng giữa các trang mượt mà |
| Bố cục không bị tràn | Đạt | Không bị dính lỗi cuộn ngang trên thiết bị di động |
| Hover / focus hoạt động | Đạt | Thẻ sản phẩm phóng to nhẹ khi di chuột, hỗ trợ bàn phím bằng `:focus-visible` |
| Đã tự sửa lỗi | Đạt | Điều chỉnh khoảng cách `gap` và `padding` cho thẻ sản phẩm trên Mobile |

---

## 6. Hướng dẫn chạy dự án
1. Tải về và giải nén tệp `my-store.zip`.
2. Mở file `index.html` bằng trình duyệt Google Chrome hoặc VS Code (Live Server).
3. Nhấn phím `F12` trên trình duyệt để kiểm tra Responsive ở các độ rộng 1366px, 768px và 390px.
