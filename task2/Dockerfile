FROM node:16-alpine

# Устанавливаем рабочую директорию
WORKDIR /home/ilovedocker/app

# Копируем скрипт hello.sh в рабочую директорию
COPY hello.sh .

# Делаем hello.sh неизменяемой командой запуска
ENTRYPOINT ["sh", "hello.sh"]
