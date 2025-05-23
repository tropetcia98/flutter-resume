# 💼 Резюме Flutter/Dart разработчика — Роман Тропин

Привет! Меня зовут **Роман Тропин**, я Flutter-разработчик из Санкт-Петербурга. Имею опыт работа в IT 3 года, разбираюсь в создании приложений с нуля, в клиент-серверной архитектуре. Разрабатываю сложное мобильное приложение с нуля, включая Telegram-авторизацию, PostgreSQL-базу, собственный Flask-сервер, управление профилем, работу с изображениями и UI-дизайн. В разработке учитываю UX, UI, сам создаю дизайн.

## Ищу работу, где пригодились бы мои навыки в flutter для раскрытия своего потенциала, становления реально крутым специалистом и финансовой стабильности, хочу расти и развиваться.
Ниже описаны мои кейсы
---

## 🚀 Ключевые навыки

- **Flutter/Dart**: кастомные UI, gestures, анимации, Bloc, drag-and-drop
- **Backend**: Flask (Python), REST API, валидации, безопасность
- **Базы данных**: PostgreSQL (self-hosted), SQLAlchemy ORM
- **Telegram Login**: OTP-авторизация через Telegram Bot API
- **Кэширование и хранение**: SharedPreferences, ExtendedImage, preload
- **UI/UX**: свайпы, зум, карточки, кастомные кнопки, неоновый стиль

## 🔐 Что реализовано в сервере (Flask + PostgreSQL). База данных

### 📌 Основные возможности:

- 🛡️ Telegram авторизация:
  - `/send_otp` — отправка OTP-кода через Telegram
  - `/verify_otp` — проверка кода
  - `/logout` — выход из аккаунта, сброс `is_verified`, сохранение `logout_at`
- 📱 Профиль:
  - `PATCH /profile` — обновление данных пользователя (анкетные поля)
  - `GET /profile` — получение всех данных профиля по номеру
- 🖼️ Фото:
  - `POST /profile/upload_photo` — загрузка фото профиля
  - `DELETE /profile/delete_photo` — удаление фото из Supabase и базы
  - `POST /profile/reorder_photos` — обновление порядка фото
  - `GET /profile/get_photos` — получение списка URL фото
- 🧹 OTP-логика:
  - Автоудаление просроченных кодов по расписанию (через `schedule`)
  - Проверка срока действия, ограничение по попыткам
- 📦 База данных:
  - Таблицы `users`, `phone_sessions`
  - Поля: `photos`, `about_me`, `profile_completion`, `telegram_user_id`, `is_verified` и т.д.
  - Типы: `UUID`, `JSONB`, `TIMESTAMP`, `Text`
  - Связь через SQLAlchemy ORM

---

### 🧠 Используемые технологии:

- `Flask`, `flask-cors` — сервер
- `SQLAlchemy`, `psycopg2` — работа с PostgreSQL
- `python-telegram-bot` — отправка сообщений, кнопки, проверка номера
- `dotenv`, `schedule`, `uuid`, `datetime`


### 🔐 Telegram авторизация

- Пользователь переходит в бота (`/start=+7...`) и делится номером
- Сервер сверяет номер → отправляет OTP → пользователь вводит код
- Авторизация и повторный вход, статус `is_verified`, logout
- SharedPreferences хранит номер и Telegram user_id

### 🖼 Фото и zoom

- До 10 фото: добавление, удаление, drag-and-drop сортировка
- Полноэкранный просмотр с pinch-to-zoom, double tap, swipe
- Кэш: `ExtendedNetworkImageProvider`, предзагрузка URL
- Визуальные эффекты: неоновая рамка, плавные переходы

### 💾 Локальное хранение

- `SharedPreferences`: номер телефона, user_id, сохранённые состояния экрана
- Используется в Telegram-авторизации, логине, logout
- Проверка и восстановление после перезапуска

### 🔁 UI и интерактив

- Bloc: состояния профиля, обновление полей, фото
- Swipe-интерфейсы: discover, анкеты, лайки
- Кнопки с эффектами: “Присоединяйся сейчас”, “Регистрация”, “Забыли пароль?”
- Debug-консоль с логами и тестированием сетевых вызовов

---

## 🧰 Стек

`Flutter` `Dart` `Python` `Flask` `PostgreSQL`  
`Bloc` `Telegram Bot API` `SharedPreferences` `ExtendedImage`  
`SQLAlchemy` `Android Studio` `VSCode` `Git`


## 📫 Контакты

- Telegram: @romanshkin

---

**Спасибо за просмотр!**  
Открыт к предложениям и сотрудничеству: full-time или проектно.
