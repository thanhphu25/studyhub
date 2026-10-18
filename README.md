# StudyHub

Dự án Django với cấu hình trong `config/` và ứng dụng `notes/`.

## Chạy trên Windows (PowerShell)

Yêu cầu Python 3.13 (phiên bản đang dùng để phát triển).

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Trang quản trị: http://127.0.0.1:8000/admin/

Tạo tài khoản quản trị bằng `python manage.py createsuperuser`.

## Khóa bí mật

Đặt biến môi trường `DJANGO_SECRET_KEY` trước khi triển khai. Khóa mặc định trong mã nguồn chỉ dành cho phát triển cục bộ. Cấu hình hiện tại bật `DEBUG` và cần được điều chỉnh trước khi triển khai thực tế.
