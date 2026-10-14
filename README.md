# Электронный Дневник 48 / Electronic Diary 48

🇷🇺 **[Русская версия ниже](#-русская-версия)** · 🇬🇧 **[English version below](#-english-version)**

---

## ⚠️ Дисклеймер / Disclaimer

**RU:** Это **не официальный дневник** и не связан с государственными системами образования (Госуслуги, Сетевой город, Дневник.ру и т.п.). Это **самостоятельный pet-проект** — демонстрация того, как может выглядеть и работать электронный дневник. **Он полностью рабочий:** авторизация, оценки, расписание, письма, годовые — всё сохраняется в базе данных и синхронизируется в реальном времени между устройствами. Но он **не является** заменой официального школьного дневника.

**EN:** This is **not an official diary** and is not affiliated with any government education systems. It is a **personal pet-project** — a demonstration of what an electronic diary could look like. **It fully works:** authentication, grades, schedule, messages, annual grades — everything is stored in a database and synced across devices in real-time. But it is **not** a replacement for an official school diary.

---

## 🇷🇺 Русская версия

### О проекте

Рабочий прототип электронного дневника для школ Липецкой области. Работает в браузере как PWA и собирается в APK для Android.

**Живая версия:** [https://angrybirdsrio07-ai.github.io/diary48/](https://angrybirdsrio07-ai.github.io/diary48/)

### Возможности

**Для учеников:**
- 📊 Просмотр оценок по предметам с датами и типом работы
- 📅 Расписание на 7 дней вперёд
- ⚖️ Средний балл по каждому предмету
- 🏆 Годовые оценки
- ✉️ Переписка с учителями
- 📝 Замечания от учителей
- 👤 Профиль со статистикой (болезни, пропуски, средний балл)

**Для учителей:**
- 📝 Журнал с оценками по классам и предметам
- ✏️ Выставление оценок (основная / дополнительная) с типом работы
- 🏆 Автоматический расчёт годовых оценок
- ✉️ Отправка писем ученикам и классам
- 📅 Личное расписание
- ⏰ Блокировка оценок через 24 часа

**Для администратора:**
- 👥 Управление пользователями (создание, редактирование, удаление)
- 🔍 Поиск по ФИО, логину, классу
- 📅 Создание расписания для любого класса
- 🔓 Разблокировка оценок

### Технологии

- **Frontend:** HTML, CSS, JavaScript (vanilla)
- **База данных:** Firebase Firestore
- **Хостинг:** GitHub Pages
- **Шрифт:** San Francisco (SF Pro Display)
- **Синхронизация:** RusDreamServer (реальное время)

### Установка

**Как PWA (на телефон):**

1. Откройте [ссылку](https://angrybirdsrio07-ai.github.io/diary48/) в браузере
2. **Android (Chrome):** меню → «Установить приложение»
3. **iPhone (Safari):** «Поделиться» → «На экран Домой»

**Как APK:**

1. Откройте [pwabuilder.com](https://www.pwabuilder.com)
2. Введите URL: `https://angrybirdsrio07-ai.github.io/diary48/`
3. **Package for Stores** → **Android** → скачать APK

### Демо-аккаунты

| Роль | Логин | Пароль |
|---|---|---|
| Администратор | `admin` | `Admin#2026` |
| Учителя | `t1` – `t11` | `Teacher#2026` |
| Ученики | `s1` – `s1652` | `School#2026` |

### Структура проекта

```
diary48/
├── index.html          # Основное приложение (всё в одном файле)
├── manifest.json       # PWA-манифест
├── icon-192.png        # Иконка для PWA
├── icon-512.png        # Иконка для PWA
├── fonts/
│   └── SF-Pro.ttf      # Шрифт San Francisco
└── README.md           # Этот файл
```

### Разработка

Проект — это **один HTML-файл** без сборки и зависимостей. Просто редактируйте `index.html` и коммитьте.

**Запуск локально:**

```bash
# Просто откройте index.html в браузере
# Или через локальный сервер:
python -m http.server 8000
```

### Лицензия

MIT

---

## 🇬🇧 English version

### About

A working prototype of an electronic diary for schools in the Lipetsk region (Russia). Works as a PWA in browsers and can be packaged as an Android APK.

**Live demo:** [https://angrybirdsrio07-ai.github.io/diary48/](https://angrybirdsrio07-ai.github.io/diary48/)

### Features

**For students:**
- 📊 View grades by subject with dates and work types
- 📅 7-day schedule
- ⚖️ Average grade per subject
- 🏆 Annual grades
- ✉️ Messages with teachers
- 📝 Remarks from teachers
- 👤 Profile with statistics (sick days, absences, average)

**For teachers:**
- 📝 Class journal by subject
- ✏️ Assign grades (main / extra) with work type
- 🏆 Automatic annual grade calculation
- ✉️ Send messages to students and classes
- 📅 Personal schedule
- ⏰ Grades lock after 24 hours

**For admin:**
- 👥 User management (create, edit, delete)
- 🔍 Search by name, login, class
- 📅 Schedule editor for any class
- 🔓 Unlock grades

### Tech stack

- **Frontend:** HTML, CSS, vanilla JavaScript
- **Database:** Firebase Firestore
- **Hosting:** GitHub Pages
- **Font:** San Francisco (SF Pro Display)
- **Sync:** RusDreamServer (real-time)

### Installation

**As PWA:**

1. Open the [link](https://angrybirdsrio07-ai.github.io/diary48/) in a browser
2. **Android (Chrome):** menu → "Install app"
3. **iPhone (Safari):** Share → "Add to Home Screen"

**As APK:**

1. Open [pwabuilder.com](https://www.pwabuilder.com)
2. Enter URL: `https://angrybirdsrio07-ai.github.io/diary48/`
3. **Package for Stores** → **Android** → download APK

### Demo accounts

| Role | Login | Password |
|---|---|---|
| Administrator | `admin` | `Admin#2026` |
| Teachers | `t1` – `t11` | `Teacher#2026` |
| Students | `s1` – `s1652` | `School#2026` |

### Project structure

```
diary48/
├── index.html          # Main app (everything in one file)
├── manifest.json       # PWA manifest
├── icon-192.png        # PWA icon
├── icon-512.png        # PWA icon
├── fonts/
│   └── SF-Pro.ttf      # San Francisco font
└── README.md           # This file
```

### Development

The project is a **single HTML file** with no build step or dependencies. Just edit `index.html` and commit.

**Run locally:**

```bash
# Simply open index.html in a browser
# Or via a local server:
python -m http.server 8000
```

### License

MIT
