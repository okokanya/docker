# Используем базовый образ Node.js версии 16 на Alpine Linux
FROM node:16-alpine

# Устанавливаем рабочую директорию внутри контейнера
WORKDIR /usr/src/app

# Копируем package.json и package-lock.json (если есть)
COPY package*.json ./

# Устанавливаем зависимости (только production-зависимости, без devDependencies)
RUN npm install --omit=dev

# Копируем все файлы проекта в рабочую директорию контейнера
COPY . .

# Открываем порт 3000 для доступа к приложению
EXPOSE 3000

# Команда, которая будет выполнена при запуске контейнера
CMD ["node", "index.js"]