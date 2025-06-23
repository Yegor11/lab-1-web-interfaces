# Майстренко Єгор КВ-41мп Програмування інтерфейсів користувача / Технологія розробки вебдодатків

## Звіти 
- Програмування інтерфейсів користувача https://docs.google.com/document/d/1JhKrS3jvdl8r3cdz6bpwLcAwXfeKyvIrgCvrbUGhCcY/edit?usp=sharing
- Tехнологія розробки Веб-додатків: https://docs.google.com/document/d/1GvXboLPOEmh_3I7YkHjXcMlvwQgNK6g1BmkGCgwrerA/edit?usp=sharing

## Функціонал
- **Аутентифікація користувача**: Реєстрація, вхід та вихід із системи.
- **Конвертація валют**: Вибір валюти, введення суми та отримання результату.
- **Історія транзакцій**: Перегляд балансу та останніх п’яти транзакцій.

## Бібліотеки
React + Vite
Django REST Framework

### Збірка

```bash
python -m venv venv
cd back
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

```bash
cd front
npm install
npm run dev
```

## 📡 АПІ

| Method | URL                         | Description                                |
|--------|-----------------------------|--------------------------------------------|
| POST   | `/exchanger/login/`         | User login, returns a token                |
| POST   | `/exchanger/register/`      | Register a new user                        |
| GET    | `/exchanger/balance/`       | Get the current user balance               |
| GET    | `/exchanger/transactions/`  | Get the latest 5 transactions              |
| POST   | `/exchanger/convert/`       | Convert currency (requires amount & types) |

