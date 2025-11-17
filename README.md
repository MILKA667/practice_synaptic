![Version](https://img.shields.io/badge/version-1.0.0-yellow)
![React](https://img.shields.io/badge/React-19.1.1-61dafb)
![Flask](https://img.shields.io/badge/Flask-3.1.2-000000)
![Docker](https://img.shields.io/badge/Docker-Ready-2496ed)

Веб-приложение для 


## 🛠 Технологии

### Frontend
- **React 19** + Vite
- **React Router DOM**

### Backend
- **Python 3.11+** + Flask
- RESTful API

### Инфраструктура
- **Docker** + Docker Compose
  
## 🌐 Сайт
**Доступно по адресу:** [BBT_RNG](http://185.237.95.6/page1)

## 📦 Установка и запуск

### Предварительные требования
- Node.js 18+ (для фронтенда)
- Python 3.11+ (для бекенда)
- Docker и Docker Compose

### Локальная разработка

#### 1. Клонируйте репозиторий
```bash
git clone https://github.com/hackathonsrus/Product_programming_binary_beasts_team_422.git
cd bbt-rng
```

#### 2. Запуск бекенда (Flask)
```bash
# Перейдите в папку бекенда
cd backend

# Создайте виртуальное окружение (рекомендуется)
python -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate  # Windows

# Установите зависимости
pip install -r requirements.txt

# Запустите Flask сервер
python app.py
```

Бекенд будет доступен на: `http://localhost:5000`

#### 3. Запуск фронтенда (в отдельном терминале)
```bash
# Вернитесь в корневую папку
cd ..
# Перейдите в папку frontend
cd frontend
# Установите зависимости
npm install

# Запустите dev сервер
npm run dev
```

Фронтенд будет доступен на: `http://localhost:5173`

### Продакшен сборка с Docker

```bash
#Клонируем репозиторий
git clone https://github.com/hackathonsrus/Product_programming_binary_beasts_team_422.git
cd Product_programming_binary_beasts_team_422

# Сборка и запуск всех сервисов
docker compose up --build

# Фоновый режим
docker compose up -d --build

# Остановка
docker compose down
```

После запуска приложение будет доступно по адресу: `http://localhost:80`


## 🐛 Поиск и устранение неисправностей

### Частые проблемы

1. **Бекенд не доступен**
   ```bash
   # Проверьте что Flask запущен
   curl http://localhost:5000/health
   ```

2. **Docker порты заняты**
   ```bash
   # Поиск процессов использующих порт
   sudo lsof -i :5000
   sudo lsof -i :80
   ```


## 👥 Авторы
