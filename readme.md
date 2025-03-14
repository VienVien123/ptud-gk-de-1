# GIỮA KÌ Blog

22003025 - NGUYỄN THỊ VIÊN


## Công nghệ sử dụng
- Django (Python Framework)
- HTML/CSS
- JavaScript (tuỳ chọn)
- Database: SQLite/PostgreSQL (tùy chọn)

## Cài đặt

### Bước 1: Clone dự án

```bash
git clone <repository-url>
cd myblog
```

## Cài đặt môi trường

Tạo và kích hoạt môi trường ảo (virtual environment):
```bash
python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows
```

Cài đặt các thư viện cần thiết:
```bash
pip install -r requirements.txt
```

## Chạy dự án

Chạy migrations để tạo database:
```bash
python manage.py migrate
```

Tạo tài khoản admin:
```bash
python manage.py createsuperuser
```

Khởi chạy server:
```bash
python manage.py runserver
```

Mở trình duyệt truy cập:
- Website: [http://localhost:8000](http://localhost:8000)
- Admin: [http://localhost:8000/admin](http://localhost:8000/admin)

## Cấu trúc dự án
```
myblog/
├── myblog/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── asgi.py
├── posts/
├── templates/
├── static/
├── user/
├── manage.py
└── db.sqlite3

```

