# Avia-Hack-2022-RealityX

### 1. Download

```
git clone https://github.com/AlexGeniusMan/Avia-Hack-2022-RealityX avia --recursive
cd avia
```

### 2. Create .env file in root directory

```
# --- Proxy ---
# - Main
PROXY_PORT=80

# --- Frontend ---
# - Main
FRONTEND_API_URL=http://localhost:80/

# --- Core Backend ---
# - Main
CORE_BACKEND_DEBUG_MODE=True
CORE_BACKEND_SECRET_KEY=YOUR_BACKEND_SECRET_KEY
CORE_BACKEND_ALLOWED_HOSTS=*
CORE_BACKEND_DEFAULT_DB=PostgreSQL
# - Default user
CORE_BACKEND_SUPERUSER_USERNAME=example@example.ru
CORE_BACKEND_SUPERUSER_EMAIL=example@example.ru
CORE_BACKEND_SUPERUSER_PASSWORD=Alpine12

# --- Database ---
# - Main
DB_HOST=db
DB_NAME=YOUR_DB_NAME
DB_USER=YOUR_DB_USER
DB_PASSWORD=YOUR_DB_PASSWORD

```

### 3. Run

```
docker-compose up --build
```

### 4. Open http://localhost:80/login

### 5. Login with `CORE_BACKEND_SUPERUSER_EMAIL` and `CORE_BACKEND_SUPERUSER_PASSWORD`