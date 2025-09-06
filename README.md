## ART Tutorial - Интернет-магазин на Vue.js 3 + Laravel

**Учебный проект** с реализацией полноценной системы аутентификации и управления товарами.

## Технологии

**Frontend:** Vue.js 3, Vite, Vue Router, Axios  
**Backend:** Laravel 10+, Sanctum, MySQL, Eloquent ORM

##  Безопасная аутентификация

-  **6-значные коды** вместо паролей
-  **Время жизни кода** - 10 минут
-  **Защита от брутфорса** - лимит 5 попыток за 30 минут
-  **Задержка между запросами** - 60 секунд
-  **Отдельная таблица** для кодов верификации

##  Возможности

-  RESTful API с JSON responses
-  Bearer token аутентификация через Sanctum
-  Form Request валидация на стороне сервера
-  Ресурсы Laravel для безопасного возврата данных
-  Сидеры для автоматического наполнения данными
-  Миграции для контроля структуры БД

## Быстрый старт

```bash
# Клонирование
git clone https://github.com/RinsL-V/ART-new.git
cd ART-new

# Бэкенд
cd backend
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan serve

# Фронтенд
npm install
npm run dev
