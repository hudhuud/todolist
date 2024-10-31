# Список задач на ExpressJs, ReactJs, NodeJs, MongoDB, SCSS

Приложение "Список задач" на основе стека MERN (MongoDB, Express, React, Node.js) с использованием SCSS для стилизации.

## Предварительный просмотр
<picture><img src="todolist/public/Todo.gif" width="100%"></picture>

## Предварительные требования

- Node.js
- npm (Node Package Manager)
- MongoDB (MongoDB Compass или MongoDB Atlas)

## Начало работы

Следуйте этим инструкциям, чтобы запустить проект на локальной машине для разработки и тестирования.

### Установка

1. Клонируйте репозиторий:

   ```bash
   https://github.com/hudhuud/todolist
   ```

2. Установите зависимости:
   ```bash
   cd todolist
   npm install
   ```

3. Запустите сервер разработки:
   ```bash
   npm run dev
   ```

4. Установите дополнительные зависимости:
   ```bash
   npm install axios react-icons
   ```

5. Настройте сервер:
   ```bash
   cd Server
   npm init -y
   npm install express mongoose cors
   ```

6. Установите Sass для поддержки SCSS:
   ```bash
   npm install sass
   ```

7. Запустите сервер:
   ```bash
   npm install nodemon
   node index.js
   ```

8. Настройте MongoDB:

   - Скачайте и установите [MongoDB Compass](https://www.mongodb.com/try/download/community) или настройте MongoDB Atlas.
   - Убедитесь, что MongoDB запущен на `mongodb://127.0.0.1:27017/TodoList`.

## Использование

- Фронтенд приложения работает на React.
- Бэкенд приложения построен на Node.js и Express.
- В качестве базы данных используется MongoDB для хранения задач.
- SCSS используется для стилизации.

## API Endpoints
- GET /get: Получить все задачи.
- PUT /update/:id: Отметить задачу как выполненную по ID.
- DELETE /delete/:id: Удалить задачу по ID.
- POST /add: Добавить новую задачу.

## Запуск приложения

1. Запустите React-сервер разработки:
   ```bash
   npm run dev
   ```

2. Запустите сервер Express:
   ```bash
   cd Server
   nodemon index.js
   ```

3. Откройте браузер и перейдите по адресу http://localhost:3000, чтобы увидеть приложение "Список задач" в действии.

## Используемые технологии

- React - библиотека JavaScript для создания пользовательских интерфейсов.
- Express - быстрый, минималистичный веб-фреймворк для Node.js.
- Node.js - среда выполнения JavaScript.
- MongoDB - NoSQL база данных для современных приложений.
- SCSS - CSS-препроцессор, добавляющий гибкость к основному языку.

## Структура файлов

```
.
├── Server
│   ├── Models
│   │   └── Todo.js
│   ├── index.js
├── public
│   └── index.html
├── src
│   ├── components
│   │   ├── Create.jsx
│   │   └── Home.jsx
│   ├── App.scss
│   ├── App.jsx
│   └── main.jsx
├── package.json
├── README.md
└── .gitignore
```

## Настройка MongoDB

1. Скачайте и установите [MongoDB Compass](https://www.mongodb.com/try/download/community) или настройте облачный экземпляр с [MongoDB Atlas](https://www.mongodb.com/products/platform/atlas-database).

2. Убедитесь, что MongoDB запущен на `mongodb://127.0.0.1:27017/TodoList`.

3. Если вы используете MongoDB Compass, создайте новую базу данных с именем `TodoList` и коллекцию с именем `todos`.
