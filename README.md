# 💼 Резюме Flutter/Dart разработчика — Роман Тропин

Привет! Меня зовут **Роман Тропин**, я Flutter-разработчик из Санкт-Петербурга.  
Имею 3 года опыта в IT, создаю мобильные приложения с нуля:  
Telegram-авторизация, PostgreSQL-база, собственный Flask-сервер, realtime-чаты на WebSocket, работа с изображениями, кастомный UI-дизайн.  
В работе учитываю UX и сам разрабатываю интерфейсы.

---

## 🔎 Цель

Ищу работу, где пригодятся мои навыки Flutter,  
чтобы расти и раскрывать свой потенциал.

---

## 🚀 Ключевые навыки

- **Flutter/Dart**: кастомные UI, Bloc, gestures, анимации, drag-and-drop
- **Realtime-чаты**: WebSocket (Flutter + Flask), сохранение сообщений
- **Backend**: Flask (Python), REST API, WebSocket, безопасность
- **Базы данных**: PostgreSQL (self-hosted), SQLAlchemy ORM
- **Telegram Login**: OTP-авторизация через Telegram Bot API
- **Кэш**: SharedPreferences, ExtendedImage, preload, offline-хранение
- **UI/UX**: discover-интерфейс, свайпы, зум, неоновые стили

---

## 🔐 Backend: Flask + PostgreSQL

### 📌 Возможности:

- **Telegram авторизация**
  - `POST /send_otp`, `POST /verify_otp`, `POST /logout`
  - Хранение `is_verified`, `logout_at`, `telegram_user_id`
- **Профиль**
  - `PATCH /profile`, `GET /profile`
- **Фото**
  - `POST /profile/upload_photo`
  - `DELETE /profile/delete_photo`
  - `POST /profile/reorder_photos`
  - `GET /profile/get_photos`
- **OTP-логика**
  - Срок действия кода, ограничение попыток
  - Автоудаление просроченных кодов (`schedule`)
- **💬 WebSocket-чаты**
  - Flask WebSocket сервер (`/ws/<user_id>`)
  - Обмен сообщениями между пользователями
  - Таблицы `chats`, `messages`, сохранение истории
  - Статусы онлайн / оффлайн (get_user_status)

---

## 🧠 Используемые технологии

`Flask` `WebSocket` `SQLAlchemy` `PostgreSQL` `python-telegram-bot`  
`schedule` `dotenv` `psycopg2` `uuid` `datetime`

---

## 📲 Telegram авторизация (OTP)

1. Пользователь переходит по ссылке вида: `https://t.me/myapp_otp_bot?start=+7...`
2. Делится номером в Telegram → сервер сохраняет
3. Пользователь вводит номер вручную в приложении
4. Сервер сверяет номера → отправляет OTP → проверка → вход

---

## 🖼 Работа с фото

- До 10 фото: загрузка, удаление, reorder
- Fullscreen просмотр: свайп, зум (pinch, double tap)
- Кэш и preload: `ExtendedNetworkImageProvider`
- Визуальные стили: неоновая рамка, плавные переходы

---

## 💾 Локальное хранилище

- `SharedPreferences`
  - Сохранение номера, `telegram_user_id`, состояний
  - Восстановление при перезапуске, логика login/logout

---

## 🔁 UI / Интерактив

- `Bloc`: логика профиля, лайков, загрузки фото
- Discover-интерфейс: свайпы, карточки пользователей
- Чаты с realtime WebSocket
- Кастомные кнопки: "Присоединяйся сейчас", "Забыли пароль?"
- Debug-консоль: логи и диагностика

---

## 🧰 Стек

`Flutter` `Dart` `Python` `Flask` `PostgreSQL`  
`Bloc` `WebSocket` `Telegram Bot API` `SharedPreferences`  
`ExtendedImage` `SQLAlchemy` `Android Studio` `VSCode` `Git`

---

## 📫 Контакты

- Telegram: [@romanshkin](https://t.me/romanshkin)

---

**Спасибо за просмотр!**  
Открыт к предложениям — full-time, part-time или проектно.
