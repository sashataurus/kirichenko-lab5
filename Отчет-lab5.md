# Лабораторная работа №5
## Введение

Создаем новый репозиторий `git-practice` и клонируем его к себе. C помощью команды `echo` создаем файл с текстом внутри. Коммитим и отправляем изменения в удаленный репозиторий:

![telegram-cloud-photo-size-2-5190625139115555971-y](https://github.com/user-attachments/assets/8e5ee245-176b-4a82-8a11-f1ce72600fe6)

Видим, что он появился на GitHub:

![аааа](https://github.com/user-attachments/assets/4759a942-db05-4663-80b6-ef2b44c6df27)

Далее создаем ветку `feature-branch`, переключаемся на неё:

![ф1](https://github.com/user-attachments/assets/b98c6b32-3f90-4349-827b-c597ee4879c0)

Меняем наш файл `example.txt` и сохраняем:

![ф2](https://github.com/user-attachments/assets/69417898-2ea9-4d6c-8fb8-7fe407e95012)

Сливаем изменения из ветки `feature-branch` в основную ветку `main`:

![2025-07-25 19 27 58](https://github.com/user-attachments/assets/b758cd25-9de3-475c-b80a-37ca37da242f)

На GitHub файл изменился, значит, всё верно.

![aaa](https://github.com/user-attachments/assets/f8e9a2cf-fdfa-4b89-a552-2db5a0878662)

## Работа с ветками

С помощью команды `touch` создаем файл `README.md` со следующим текстом внутри:

![telegram-cloud-photo-size-2-5190625139115556143-x](https://github.com/user-attachments/assets/a021504c-39fe-417e-9230-c9c03a8f6e55)

Затем создаю новую ветку `feature-login`:

![2025-07-25 19 39 56](https://github.com/user-attachments/assets/740dfe49-8703-4f02-bcc1-8a96b05e3eee)

Изменяем файл и сохраняем изменения:

![2025-07-25 19 46 57](https://github.com/user-attachments/assets/48389369-8bcf-403f-8454-d1a97bf5aeba)
![2025-07-25 19 39 56 — копия](https://github.com/user-attachments/assets/9cb28c45-7eb0-41f2-afce-8997f8c95b51)

Видим, что на GitHub всё отобразилось:

![telegram-cloud-photo-size-2-5190625139115556182-y](https://github.com/user-attachments/assets/f61ebfc4-f52c-40a2-84b4-fd8ee2bd8f96)

## Работа с удаленным репозиторием

Переключаемся на основную ветку, вносим изменения в файл и коммитим. Видим, что на GitHub всё верно:

![2025-07-25 19 46 51](https://github.com/user-attachments/assets/1b325f46-8349-4542-9127-c1c0e572d9a5)
![2025-07-25 19 46 45](https://github.com/user-attachments/assets/801b7432-d5ad-4c6e-bdcc-e2f6cccafaef)
![telegram-cloud-photo-size-2-5190625139115556181-y](https://github.com/user-attachments/assets/73c4f214-eb29-4afb-943b-d07b7c5ae1e3)

## Моделирование конфликта

Переключаемся на ветку `feature-login`, вносим изменения в файл во 2 главу и коммитим:

![2025-07-25 19 54 52](https://github.com/user-attachments/assets/d331b58e-8deb-448d-be9e-6cc2d3f087f5)
![2025-07-25 19 54 55](https://github.com/user-attachments/assets/39959cf0-87f7-47ea-a590-de8dad6268cb)

## Разрешение конфликта

Возвращемся в основную ветку и пробуем слить изменения. Возникает конфликт:

![2025-07-25 20 03 09](https://github.com/user-attachments/assets/6c4a11b2-178f-49a4-9fdb-06d0bbd92b4b)

Меняем содержимое файла, удаляя из него лишние метки:

![2025-07-25 20 04 24](https://github.com/user-attachments/assets/c101221f-4c2f-4be8-a429-676779b7ec9b)
![2025-07-25 20 04 27](https://github.com/user-attachments/assets/2d98b76b-e297-4709-9e4d-c625301cc53d)

Коммитим разрешение конфликта и отправляем изменения на GitHub. Всё в порядке.

![telegram-cloud-photo-size-2-5190625139115556271-x](https://github.com/user-attachments/assets/fcff897e-9a3d-4f08-80a1-4c02b46af08c)
![telegram-cloud-photo-size-2-5190625139115556265-y](https://github.com/user-attachments/assets/6f661593-0d6f-4953-8b45-940896376f21)

## Автоматизация проверки формата файлов при коммите

Создаем bash-скрипт `pre-commit`, который выполняет проверку формата `.txt` файлов:

![telegram-cloud-photo-size-2-5190625139115556307-x](https://github.com/user-attachments/assets/c15c969e-c031-4b9f-963a-ae73168aa4cd)

описание скрипта

Добавляем его в папку `.git/hooks`.



