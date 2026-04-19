React Docker App "ToDoList"
Простое React-приложение "список задач", запущенное в Docker-контейнере с использованием Nginx.


Запуск проекта
1. Сборка Docker-образа
 docker build -t my-react-app .
2. Запуск контейнера
 docker run -d -p 8080:80 --name my-app my-react-app


Открыть в браузере по адресу:
http://localhost:8080

Что будет на экране:
![](2026-04-19-11-29-28.png)


Структура проекта
app/ — React-приложение
Dockerfile — сборка контейнера
nginx.conf — конфигурация nginx
.dockerignore — исключения файлов


Дополнительно
Проект использует:
 - multi-stage Docker build
 - nginx для раздачи статики
 