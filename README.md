# 1. Check the version of Python
## Windows
```bash
python --version
```

## Linux
```bash
python3 --version
```

# 2. Create virtual enviroment
## Windows
```bash
python -m venv venv
```

## Linux
```bash
python3 -m venv venv
```

# 3. Activate virtual enviroment
## Windows
```bash
venv\Scripts\activate
```

### IF an error occurs "execution policy", please run:
```bash
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```

## Linux
```bash
source venv/bin/activate
```

# 4. Install framework
```bash
pip install -U pip
pip install -r requirements.txt
```

# 5. Check framework
```bash
pip list
```

# 6. Thoát môi trường ảo
```bash
deactivate
```

# 7. Xóa hoặc làm mới môi trường (khi cần)
```bash
rm -rf venv          # Linux / macOS
rmdir /s /q venv     # Windows CMD
```



<hr>
Bước 1: Đâu tiên chạy file "split_data"
Bước 2: Sau đó  vào thư mục problem để lấy 1 số bức ảnh sang bên public_test và private_test
Lưu ý: Ảnh ở 3 thư mục problem và public_test và private_test không được trùng nhau
Bước 3: Vào file main để chạy chương trình chính