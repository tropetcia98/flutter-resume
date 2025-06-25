# 💼 Резюме Flutter/Dart разработчика — Роман Тропин

Привет! Меня зовут **Роман Тропин**, я Flutter-разработчик из Санкт-Петербурга.  
Имею 3 года опыта в IT: участвовал в разработке коммерческих и собственных мобильных приложений.  
Реализую весь цикл: от дизайна интерфейсов и бизнес-логики до серверной части и публикации.

- В команде разработчиков приложения **Музей РЖД** (2022 – февраль 2025):  
  работал над экранами, навигацией, бизнес-логикой, интеграцией с AR и настройкой билдов.

- В настоящее время веду собственный проект: Flutter-клиент + Flask-сервер с Telegram-авторизацией, PostgreSQL-базой, realtime-чатами, кастомной UI/UX-системой.

---

## 🔎 Цель

Ищу интересные **проекты на Flutter**, в которых можно применять как технические, так и продуктовые навыки.  
Готов к участию в **проектной, part-time или full-time** разработке — как в команде, так и самостоятельно.

---

## 🚀 Ключевые навыки

- **Flutter/Dart**: кастомные UI, Bloc, gestures, анимации, drag-and-drop
- **Realtime-чаты**: WebSocket (Flutter + Flask), сохранение истории
- **Backend**: Flask (Python), REST API, WebSocket, безопасность
- **Базы данных**: PostgreSQL (self-hosted), SQLAlchemy ORM
- **Telegram Login**: OTP-авторизация через Telegram Bot API
- **Кэш и хранилище**: SharedPreferences, ExtendedImage, offline-режим
- **UI/UX**: discover-интерфейс, свайпы, зум, неоновые стили, AR-модули

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
  - Срок действия, ограничение попыток, автоудаление (schedule)
- **💬 WebSocket-чаты**
  - Обмен сообщениями между пользователями
  - Таблицы `chats`, `messages`, статусы онлайн/оффлайн

---

## 🧠 Используемые технологии

`Flutter` `Dart` `Python` `Flask` `PostgreSQL`  
`SQLAlchemy` `WebSocket` `Telegram Bot API`  
`SharedPreferences` `ExtendedImage` `uuid` `dotenv` `schedule`

---

## 📲 Telegram авторизация (OTP)

1. Пользователь переходит по ссылке `https://t.me/myapp_otp_bot?start=+7...`
2. Делится номером → сервер сохраняет
3. Вводит номер в приложении → сверка → отправка OTP → проверка → вход

---

## 🖼 Работа с фото

- До 10 фото: загрузка, удаление, reorder
- Fullscreen просмотр: свайп, зум (pinch, double tap)
- Кэш и preload: `ExtendedNetworkImageProvider`
- UI: неоновые рамки, плавные переходы

---

## 💾 Локальное хранилище

- `SharedPreferences`
  - Хранение номера, `telegram_user_id`, состояний
  - Логика login/logout, восстановление при запуске

---

## 🔁 UI / Интерактив

- `Bloc`: логика профиля, лайков, загрузки фото
- Discover-интерфейс: свайпы, карточки
- Чаты на WebSocket
- Кастомные кнопки: "Присоединяйся сейчас", "Забыли пароль?"
- Встроенная debug-консоль

---

## 🧰 Инструменты и стек

`Flutter` `Dart` `Python` `Flask` `PostgreSQL`  
`Bloc` `WebSocket` `Telegram Bot API` `SharedPreferences`  
`ExtendedImage` `Android Studio` `VSCode` `Git`

---

## 📫 Контакты

- Telegram: [@romanshkin](https://t.me/romanshkin)

---

**Спасибо за просмотр!**  
Открыт к предложениям — проектная работа, part-time или full-time.
