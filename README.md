# TikTok Data Visualizer

![Приложение](https://github.com/user-attachments/assets/80698d91-97e9-4cae-9177-3dbff2292d07)

## 📱 О проекте

TikTok Data Visualizer - это веб-приложение для анализа и визуализации истории чатов из экспортированных данных TikTok. Приложение позволяет загрузить JSON-файл с историей переписки и отображает подробную статистику вашего общения.

## ✨ Возможности

- Загрузка и анализ JSON-файлов с историей чатов TikTok
- Отображение списка пользователей, с которыми вы общались
- Подробная статистика для каждого чата:
  - Общее количество сообщений
  - Среднее количество сообщений в день
  - Распределение сообщений между участниками
  - Наиболее часто используемые слова
  - Активность общения по датам

## 🛠 Технологии

- **Frontend**: HTML, CSS, JavaScript, Chart.js
- **Backend**: Node.js, Express
- **Дополнительные библиотеки**: Moment.js, Lodash

## 🚀 Установка и запуск

### Требования

- Node.js (версия 14 или выше)
- npm (устанавливается вместе с Node.js)
- экспортированные сообщения TikTok в формате JSON (Подробнее в разделе "как использовать")
- для хостинга в production требуется установить { secure: true } в настройке сессий

### Шаги установки

1. Клонируйте репозиторий:

```bash
git clone https://github.com/your-username/tiktok-data-visualizer.git
cd tiktok-data-visualizer/chat-analyzer
```

2. Установите зависимости:

```bash
npm install
```

3. Запустите сервер:

```bash
npm start
```

4. Откройте в браузере http://localhost:3000

## 📖 Как использовать

1. **Экспортируйте данные из TikTok**:

   - Откройте TikTok на мобильном устройстве
   - Перейдите в настройки → Аккаунт → Скачать ваши данные
   - выберите только сообщения для скачивания
   - Выберите "JSON" в качестве формата экспорта
   - Дождитесь, пока данные будут готовы к скачиванию

2. **Работа с приложением**:
   - Загрузите полученный JSON-файл через форму на главной странице
   - Выберите пользователя из списка слева
   - Просмотрите подробную статистику общения

## 🧩 Структура проекта

tiktok-data-visualizer/
├── chat-analyzer/
│ ├── public/
│ │ ├── css/
│ │ ├── js/
│ │ └── index.html
│ ├── server.js
│ └── package.json
└── README.md
