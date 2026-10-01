# BookNest — onlayn kutubxona platformasi

## Ishga tushirish

```bash
pip install -r requirements.txt

py manage.py makemigrations catalog
py manage.py migrate
py manage.py createsuperuser
py manage.py runserver
```

Keyin brauzerda:

- Katalog: http://127.0.0.1:8000/
- Admin panel (jazzmin): http://127.0.0.1:8000/admin/
- Kirish sahifasi: http://127.0.0.1:8000/login/

## Birinchi ma'lumotlarni qo'shish

Admin panelga superuser bilan kiring, so'ng navbat bilan qo'shing:

1. **Genre** (janrlar) — masalan: Roman, Fantastika, Tarix
2. **Author** (mualliflar)
3. **Book** (kitoblar) — muqova rasm yuklaganingizda, Pillow avtomatik
   thumbnail (`cover_thumbnail`) yaratadi

Oddiy foydalanuvchi (superuser emas) `/login/` orqali kirib, kitoblarga
sharh qoldirishi va o'qish ro'yxatiga qo'sha oladi.

## Loyiha tuzilishi

```
booknest/
├── manage.py
├── booknest/          # loyiha sozlamalari (settings.py, urls.py)
├── catalog/            # asosiy ilova (models, views, admin, forms)
├── templates/           # HTML shablonlar (kartoteka-kartochka dizayni)
└── static/              # CSS/JS
```
