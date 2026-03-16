# Kittygram Backend

## Запуск проекта локально

### 1. Клонируй репозиторий и перейди в него
```bash
git clone https://github.com/pademirov/kittygram_backend.git
cd kittygram_backend
```

### 2. Создай и активируй виртуальное окружение

**Windows:**
```bash
python -m venv env
env\Scripts\activate
```

**Mac / Linux:**
```bash
python3 -m venv env
source env/bin/activate
```

### 3. Обнови pip и установи зависимости
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Примени миграции
```bash
python manage.py migrate
```

### 5. Запусти сервер
```bash
python manage.py runserver
```

После этого проект будет доступен по адресам: http://127.0.0.1:8000/ и http://localhost:8000/

## Зависимости

| Пакет | Версия | Назначение |
|---|---|---|
| Django | 5.1.1 | Основной фреймворк |
| djangorestframework | 3.15.2 | REST API |
| djoser | 2.3.1 | Аутентификация и управление пользователями |
| djangorestframework_simplejwt | 5.5.1 | JWT-токены |
| django-cors-headers | 4.9.0 | Обработка CORS-заголовков |
| pillow | 11.0.0 | Работа с изображениями |
| webcolors | 1.11.1 | Конвертация HEX-цветов в названия |
| social-auth-app-django | 5.7.0 | Авторизация через соцсети |
| gunicorn | 21.2.0 | WSGI-сервер для продакшна |
| python-dotenv | 1.0.1 | Загрузка переменных из .env файла |
| requests | 2.32.5 | HTTP-запросы |
| asgiref | 3.11.1 | ASGI-совместимость |
| sqlparse | 0.5.5 | Парсинг SQL-запросов |

Полный список зависимостей с версиями — в файле `requirements.txt`.