# Học liệu Toán tương tác — THPT

**Trang web: https://hlinhmar.github.io/bgdt_ln/**

Bộ **11 bài giảng điện tử** môn Toán lớp 10 và 11, biên soạn theo Chương trình Giáo dục phổ thông 2018.

Mỗi bài là **một file HTML độc lập**: mở bằng trình duyệt bất kỳ, chiếu lên máy chiếu hoặc gửi cho học sinh tự học. Không cần tài khoản, không cần cài phần mềm, không phụ thuộc mạng sau lần tải đầu tiên.

## Danh sách bài giảng

### Toán 10

| Bài | Nội dung chính |
|---|---|
| [Mệnh đề](BaiGiangMenhDe.html) | Mệnh đề, phủ định, kéo theo, tương đương, mệnh đề chứa biến |
| [Số gần đúng và Sai số](BaiGiang_SoGanDung.html) | Sai số tuyệt đối, sai số tương đối, quy tắc quy tròn |
| [Mô tả và Biểu diễn Dữ liệu](BaiGiang_MoTaDuLieu_lop10.html) | Bảng số liệu, biểu đồ cột, biểu đồ quạt |
| [Đường Elip](BaiGiangElip.html) | Phương trình chính tắc, tiêu điểm, tâm sai |
| [Đường Hypebol](BaiGiangHypebol.html) | Hai nhánh, tiệm cận, phương trình chính tắc |
| [Đường Parabol](BaiGiangParabol.html) | Tiêu điểm, đường chuẩn, tham số tiêu |

### Toán 11

| Bài | Nội dung chính |
|---|---|
| [Điểm, Đường thẳng và Mặt phẳng](BaiGiang_DiemDuongMat.html) | Sáu tính chất thừa nhận, xác định mặt phẳng, hình chóp, tứ diện |
| [Hai Đường Thẳng Song Song](BaiGiang_2DTSS.html) | Vị trí tương đối trong không gian, tính chất và định lí |
| [Lũy thừa với Số mũ thực](BaiGiang_Luythua.html) | Số mũ hữu tỉ và vô tỉ, lãi kép, tăng trưởng |
| [Phép tính Lôgarit](BaiGiang_PhepTinhLogarit.html) | Công thức biến đổi, đổi cơ số, thang Richter |
| [Phương trình và Bất phương trình Mũ – Lôgarit](BaiGiang_PTMuLoga.html) | Phương pháp giải theo dạng, điều kiện xác định |

## Tính năng chung của mọi bài

- **Applet tương tác** — kéo thanh trượt để thấy đồ thị biến đổi theo tham số
- **Mô hình 3D** — xoay hình chóp, tứ diện bằng chuột (các bài hình học không gian)
- **Flashcards và game kéo thả** — củng cố ghi nhớ công thức
- **Trắc nghiệm phân tầng** — nhận biết, thông hiểu, vận dụng; phản hồi và giải thích ngay sau mỗi câu
- **Tự lưu bài làm** — kết quả trắc nghiệm được giữ trong trình duyệt, mở lại vẫn còn; có nút *Làm lại*
- **Điều hướng liên bài** — thanh *Về thư viện* và nút *Bài trước / Bài sau* theo mạch kiến thức
- **Trợ năng** — chế độ tương phản cao, điều hướng đầy đủ bằng bàn phím, skip-link, bố cục đọc tốt trên điện thoại
- **Chế độ sáng / tối** trên trang thư viện

## Cấu trúc thư mục

```
.
├── index.html              # Trang thư viện: tìm kiếm, lọc theo khối lớp, chế độ tối
├── 404.html                # Trang báo lỗi, dẫn về thư viện
├── BaiGiang*.html          # 11 bài giảng, mỗi file chạy độc lập
├── favicon.svg
├── og-image.png            # Ảnh xem trước khi chia sẻ link
├── sitemap.xml             # Danh mục URL cho công cụ tìm kiếm
├── robots.txt
├── .nojekyll               # Tắt Jekyll để GitHub Pages phục vụ file nguyên trạng
├── netlify.toml            # Chỉ dùng nếu chuyển sang Netlify; GitHub Pages bỏ qua file này
└── _backup/                # Bản gốc trước khi chỉnh — KHÔNG đẩy lên Git (xem .gitignore)
```

## Công nghệ

HTML, CSS và JavaScript thuần, không framework, không bước build. Chỉ dùng ba thư viện qua CDN:

- [MathJax 3](https://www.mathjax.org/) — hiển thị công thức toán
- [Font Awesome 6](https://fontawesome.com/) — biểu tượng
- [Google Fonts](https://fonts.google.com/) — Merriweather và Nunito

## Chạy thử trên máy

Mở trực tiếp `index.html` bằng trình duyệt là đủ. Nếu muốn chạy qua máy chủ cục bộ:

```bash
python3 -m http.server 8000
# rồi mở http://localhost:8000
```

## Ghi chú khi triển khai

- Ảnh xem trước (`og:image`) đang để **đường dẫn tương đối**. Hầu hết nền tảng (Facebook, Zalo, Messenger) tự phân giải được. Nếu muốn chắc chắn tuyệt đối, đổi thành URL đầy đủ sau khi có tên miền, ví dụ `https://ten-site.netlify.app/og-image.png`.
- Thư mục `_backup/` đã được `.gitignore` loại trừ. **Không gỡ dòng đó** — các file trong đó là bản chưa dọn.

## Giấy phép

Học liệu phục vụ mục đích giáo dục phi lợi nhuận. Giáo viên được tự do sử dụng, chỉnh sửa và chia sẻ cho hoạt động dạy học.
