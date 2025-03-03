FROM node:16-alpine

# Устанавливаем рабочую директорию
WORKDIR /home/ilovedocker/app

# Копируем скрипт hello.sh в рабочую директорию
COPY hello.sh .

# Устанавливаем команду запуска (неизменяемую)
CMD ["sh", "hello.sh"]