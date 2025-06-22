# ДР к занятию 4 «Оркестрация группой Docker контейнеров на примере Docker Compose»

## Решение задачи 1
Ссылка в dockerhub-репозиторий:
[mspitsyn/custom-nginx](https://hub.docker.com/repository/docker/mspitsyn/custom-nginx/general)

## Решение задачи 2
[task-2](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-2.png)
[task-2-1](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-2-1.png)

## Решение задачи 3
[task-3](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-3.png)
[task-3-1](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-3-1.png)
[task-3-2](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-3-1.png)

## Решение задачи 4
[task-4](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-4.png)

## Решение задачи 5
5.1. Создал 2 файла с содержимым из задания
Выполнил команду: ```docker compose up -d```
Был запущен файл compose.yaml. Т.к. если оба файла существуют, Docker Compose предпочитает канонический compose.yaml.

5.2. 
```yaml
version: "3"
include:
  - docker-compose.yaml
services:
   portainer:
     image: portainer/portainer-ce:latest
     ports:
       - "9000:9000"
     volumes:
       - /var/run/docker.sock:/var/run/docker.sock
```
5.3. [task-5.3](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-5-3.png)
5.4. [task-5.4](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-5-4.png)
5.5. [task-5.5](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-5-5.png)
5.6. [task-5.6](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-5-6.png)
5.7. [task-5.7](https://github.com/mspitsyn/04-docker-intro/blob/main/screenshots/task-5-7.png)