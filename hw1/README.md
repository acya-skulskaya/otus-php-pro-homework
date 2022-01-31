# Работа с окружением
Цель:
Познакомиться с различными типами организации окружения. Осознать их применимость и необходимость. Научиться настраивать рабочее окружение для своих проектов с использованием автоматизации.

1. Docker

1. Установить Docker себе на локальную машину

2. Описать инфраструктуру в Docker-compose, которая включает в себя

2. 2.1. nginx (обрабатывает статику, пробрасывает выполнение скриптов в fpm)

3. 2.2. php-fpm (соединяется с nginx через unix-сокет)

4. 2.3. redis (соединяется с php по порту)

5. 2.4. memcached (соединяется с php по порту)

3. БД подключать как отдельную VM (можно на базе Homestead), либо как контейнер (но тогда не забудьте про директории с данными)

6. Виртуальные машины.

1. Развернуть Homestead VM при помощи Vagrant и VirtualBox

2. Сайт должен отвечать на доменное имя application.local

3. Должна быть поддержка проброса директорий

Критерии оценки:

Каждый RUN в Dockerfile будет создавать промежуточный образ при сборке. Помните об этом. Желательно снизить их использование до минимума.