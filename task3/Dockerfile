FROM node:16-alpine

# Устанавливаем рабочую директорию
WORKDIR /home/ilovedocker/app

# Копируем package.json и package-lock.json (если есть)
COPY package*.json ./

# Устанавливаем зависимости
RUN npm install --only=production

# Копируем весь исходный код проекта
COPY . .

# Экспонируем порт 3032
EXPOSE 3032

# Запускаем main.js с помощью node
ENTRYPOINT ["node", "main.js"]
