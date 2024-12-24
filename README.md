# Hệ thống Quản lý Học tập

## Chạy cục bộ

1. Sao chép dự án

```bash
git clone https://github.com/nz-m/eLMS-SWE.git
```

2. Đi đến thư mục dự án

```bash
cd eLMS-SWE
```

3. Tạo môi trường ảo và kích hoạt nó (Windows)

```bash
python -m venv env
```

```bash
env\Scripts\activate
```

4. Cài đặt các phụ thuộc

```bash
pip install -r requirements.txt
```

> **Lưu ý:** Nếu bạn đang sử dụng các phiên bản python mới hơn (3.10+), bạn có thể cần thêm tùy chọn `--use-deprecated=legacy-resolver` khi cài đặt các phụ thuộc với `pip` để tránh lỗi:

```bash
pip install -r requirements.txt --use-deprecated=legacy-resolver
```

5. Tạo các di chuyển và di chuyển

```bash
python manage.py makemigrations
```

```bash
python manage.py migrate
```

6. Tạo admin/superuser

```bash
python manage.py createsuperuser
```

7. Cuối cùng chạy dự án

```bash
python manage.py runserver
```

Bây giờ dự án sẽ chạy trên http://127.0.0.1:8000/

Đăng nhập với tư cách quản trị viên và thêm một số khóa học, giáo viên và sinh viên.