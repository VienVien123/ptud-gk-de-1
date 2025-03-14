# Blog Project - Midterm

**MSSV:** 22003025  
**Họ và tên:** NGUYỄN THỊ VIÊN

## Chức năng chính
- **Bình luận (Comment)** với các vai trò phân quyền:
  - **Viewer**: Chỉ có thể xem.
  - **Collaborator**: Có thể chỉnh sửa, nhưng không thể xóa.
  - **Editor**: Có quyền xem, chỉnh sửa, và xóa.

## Công nghệ sử dụng
- **Framework:** Django (Python)
- **Front-end:** HTML/CSS, JavaScript (tùy chọn)
- **Database:** SQLite hoặc PostgreSQL

## Hướng dẫn cài đặt

### Bước 1: Clone dự án

```bash
git clone <repository-url>
cd myblog
```

### Bước 2: Thiết lập môi trường ảo

Tạo môi trường ảo:

- **Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

- **Linux/macOS:**
```bash
python -m venv venv
source venv/bin/activate
```

### Bước 3: Cài đặt dependencies

```bash
pip install -r requirements.txt
```

### Bước 4: Thiết lập Database

Chạy migrations:
```bash
python manage.py migrate
```

Tạo tài khoản admin:
```bash
python manage.py createsuperuser
```

### Bước 5: Khởi động server

```bash
python manage.py runserver
```

## Truy cập ứng dụng

- **Trang web chính:** [http://localhost:8000](http://localhost:8000)
- **Trang admin:** [http://localhost:8000/admin](http://localhost:8000/admin)

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


