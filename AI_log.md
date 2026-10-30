không hiện ảnh 
không đúng đường dẫn
## Ghi nhận lỗi

1. **Ảnh minh họa dự án không hiển thị**
	- Vị trí: `index.html`, ba thẻ ảnh trong mục `#du-an`.
	- Hiện trạng: đường dẫn lần lượt là `asset/du-an-1.jpg`, `asset/du-an-2.jpg`, `asset/du-an-3.jpg`.
	- Nguyên nhân quan sát được: trang dùng thư mục `asset/` (số ít), nhưng trong dự án chỉ có `assets/` (số nhiều), và thư mục `assets/` hiện chỉ có `download.jpg`. Ba tệp ảnh dự án không tồn tại nên trình duyệt không tải được.
	- Cách kiểm tra lại: mở `index.html`, cuộn tới mục **Dự án**, xác nhận cả ba ảnh bị lỗi; trong DevTools > Network có thể thấy yêu cầu ảnh trả về 404.
	- Hướng xử lý: đặt đúng các ảnh dự án vào thư mục được chọn và cập nhật `src` cho khớp tên/thư mục; sau đó tải lại trang và xác nhận cả ba ảnh hiển thị.

2. **Tên hiển thị chưa thống nhất**
	- Vị trí: `index.html` phần giới thiệu hiển thị “Cao Thăng”; `kiem-tra-lab5.txt` ghi họ tên “Kiều Cao Thăng”.
	- Cần xác nhận tên chính xác với tác giả rồi thống nhất giữa hồ sơ và trang portfolio.
