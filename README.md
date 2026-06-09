# Clicker Game — Flask Web Application

Веб-приложение на основе Flask с системой регистрации и авторизации пользователей. Разработано в рамках курса по веб-разработке на ZeroCoder.

## Стек технологий

- **Python 3.x**
- **Flask** — веб-фреймворк
- **Flask-SQLAlchemy** — ORM для работы с базой данных
- **Flask-Login** — управление сессиями пользователей
- **Flask-WTF** — работа с формами
- **SQLite** — база данных
- **Bootstrap** — стилизация интерфейса

## Структура проекта

```
clicker-game/
├── app/
│   ├── __init__.py       # Инициализация приложения Flask
│   ├── models.py         # Модели базы данных (User)
│   ├── forms.py          # Формы регистрации и входа
│   ├── routes.py         # Маршруты и логика приложения
│   └── templates/
│       ├── base.html     # Базовый шаблон
│       ├── index.html    # Главная страница
│       ├── login.html    # Страница входа
│       └── register.html # Страница регистрации
├── main.py               # Точка входа приложения
├── .gitignore
└── README.md
```

## Локальный запуск проекта

### 1. Клонирование репозитория

```bash
git clone https://github.com/IrinaZeroDev/clicker-game.git
cd clicker-game
```

### 2. Создание виртуального окружения

```bash
python -m venv .venv
```

Активация:
- **Windows:** `.venv\Scripts\activate`
- **macOS / Linux:** `source .venv/bin/activate`

### 3. Установка зависимостей

```bash
pip install flask flask-sqlalchemy flask-login flask-wtf
```

### 4. Запуск приложения

```bash
python main.py
```

После запуска приложение будет доступно по адресу: [http://127.0.0.1:5000](http://127.0.0.1:5000)

## Развёртывание на PythonAnywhere

1. Зарегистрироваться на [pythonanywhere.com](https://www.pythonanywhere.com/)
2. В разделе **Web** создать новое веб-приложение (Flask, Python 3.12)
3. Указать путь к основному файлу: `/home/<username>/mysite/main.py`
4. Через раздел **Files** загрузить файлы проекта в папку `mysite/`
5. В `main.py` убедиться, что присутствует строка `with app.app_context(): db.create_all()`
6. Нажать кнопку **Reload** в разделе Web

## Демо

Проект развёрнут и доступен по адресу: [https://vgomoz62.pythonanywhere.com](https://vgomoz62.pythonanywhere.com)
