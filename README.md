# DOCKER + NGINX + PHP

## Описание проекта

Проект состоит из двух контейнеров:
- контейнер проекта с предустановленным PHP-fpm 8.2
- контейнер с nginx

## Работа с проектом

Локальный домен: ``http://localhost:8081``

Установлен Xdebug v3.2.0. Настраивается стандартно, никаких доп. действий по настройке не требуется.

Посмотри ``Makefile`` - там описаны основные операции (сборка проекта, запуск проекта и т.д.)

## Архитектура проекта
Проект имеет примитивную архитектуру:
- конфигурационные файлы докер образа проекта находятся внутри дирриктории ``docker``
- публичные файлы проета находятся в дирректории ``public``
- исполнительные файлы проекта рекомендуется добавлять в дирректорию ``src``

## Устновка проекта
1. Скачать проект
2. Выполнить команду ``make docker-build``