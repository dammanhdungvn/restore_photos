## Restore Photos – Tài liệu dự án

### Mục đích
Project này nhằm giải quyết bài toán xử lý/khôi phục ảnh và tổ chức dữ liệu phục vụ bài thi. Người dùng có thể:
- Chuẩn bị dữ liệu (chia ảnh, tổ chức thư mục train/test)
- Chạy thuật toán chính để tạo kết quả đầu ra

Lưu ý quan trọng theo yêu cầu dự án:
- `topic_2025/` là thư mục chứa đề bài thi
- `images/docs/` là nơi lưu một số ảnh demo kết quả/sản phẩm

### Cấu trúc thư mục chính
- `code/`
	- `main.ipynb`: Notebook chính để chạy pipeline/thuật toán
	- `split_images.ipynb`: Notebook hỗ trợ tách/chuẩn bị dữ liệu
- `images/`
	- `problem/` (dữ liệu gốc theo đề, có thể chia theo `task1/`, `task2/`)
	- `public_test/`, `private_test/` (ảnh test công khai/riêng tư để đánh giá)
	- `docs/` (ảnh demo minh họa sản phẩm)
- `output/`
	- `permutations/` (ví dụ các file JSON kết quả trung gian/đầu ra)
- `topic_2025/` (đề bài thi)
- `requirements.txt` (danh sách thư viện Python)

### Hướng dẫn nhanh (Quick start)
1) Tạo môi trường và cài thư viện
	 - Linux/macOS:
		 ```bash
		 python3 -m venv venv
		 source venv/bin/activate
		 pip install -U pip
		 pip install -r requirements.txt
		 ```
	 - Windows (PowerShell):
		 ```bash
		 python -m venv venv
		 venv\Scripts\activate
		 pip install -U pip
		 pip install -r requirements.txt
		 ```

2) Chuẩn bị dữ liệu
	 - Mở `code/split_images.ipynb` và chạy các ô lệnh theo hướng dẫn để tách/chuẩn bị dữ liệu.
	 - Di chuyển/chọn một số ảnh từ `images/problem/` sang `images/public_test/` và `images/private_test/` để làm bộ test.
	 - Lưu ý: Ảnh trong ba thư mục `images/problem/`, `images/public_test/`, `images/private_test/` KHÔNG được trùng nhau.

3) Chạy thuật toán chính
	 - Mở `code/main.ipynb` và chạy lần lượt các ô lệnh để tạo kết quả.
	 - Kết quả có thể được ghi vào `output/` (ví dụ: `output/permutations/*.json`).

### Gỡ lỗi nhanh
- Kiểm tra phiên bản Python:
	```bash
	python3 --version
	```
- Kiểm tra gói đã cài:
	```bash
	pip list
	```
- Thoát môi trường ảo khi cần:
	```bash
	deactivate
	```
- Xóa môi trường ảo (khi cần làm sạch):
	```bash
	rm -rf venv          # Linux / macOS
	rmdir /s /q venv     # Windows CMD
	```

### Ghi chú
- `images/docs/` chỉ mang tính minh họa kết quả, không dùng làm dữ liệu train/test.
- Nếu có thay đổi cấu trúc dữ liệu, hãy cập nhật lại đường dẫn trong các notebook tương ứng.