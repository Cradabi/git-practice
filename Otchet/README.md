# Отчет по лабораторной работе №5
## Введение
Клонируем репозиторий и создаем файл example.txt, куда вписываем произвольный текст. И данный файл отправляем в ветку main.
![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20003920.png)

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20004354.png)

Создаем новую ветку, меняем файл example.txt и загружаем обновленный файл на GitHub.
![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20004729.png)

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20005949.png)

Затем переходим в ветку main и соединяем изменения. Пушим полученное.
![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20010735.png)

Проверяем, что в проекте есть 2 ветки и в ветке main лежит файл из второй ветки.
![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20010935.png)

## Раабота с ветками

Создаем новый файл с произвольным текстом.
![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20011543.png)

Создаем новую ветку feature-login, переходим туда, изменяем новый файл и пушим измененный файл.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20011818.png)

## Работа с удаленным репозиторием

Переходим в ветку main.
Изменяем файл example.txt и отправляем на GitHub.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20013113.png)

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20013532.png)

## Моделирование конфликта

Переходим в ветку feature-login и изменяем файл так, чтобы он отличался от того, который лежит в ветке main. После этого отправляем измененный файл на GitHub.
![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20013818.png)

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20014005.png)

## Разрешение конфликта

Переходим в ветку main. Пытемся слить ветки и получаем сообщение о конфликте.
![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20014854.png)

Для разрешения конфликта меняем файл, после чего коммитим и пушим файл в ветку main без конфликтов.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20014941.png)

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20015015.png)

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20015150.png)

## Автоматизация проверки формата файлов при коммите

Создаем bash-script, который будет проходиться по всем файлам репозитория и проверять, есть ли указанная строчка в файле.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20024258.png)

Даем файлу право на выполнение. И запускаем скрипт.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20022918.png)

Такие файлы были созданы для тестов.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20022950.png)

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20023014.png)

Далее видим что при создании коммита он не выполняется, если все файлы не проходят проверку.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20024453.png)

Меняем все файлы, чтобф они подходили под правильный формат и создаем коммит.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20024802.png)

## Использование Git Flow в проекте

Инициализируем Git Flow и создаем ветку для новой функциональности "task-management".
Создаем файл task_manager.py.
Создаем коммит и закрываем фичу.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20030256.png)

Переключаемся на ветку "develop" и начинаем создание релиза.
Изменяем файл version.txt и коммитим его.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20030804.png)

Заканчиваем релиз.

![Image alt](https://github.com/Cradabi/git-practice/blob/main/Снимок%20экрана%202023-12-26%20031045.png)

## Вывод
Во время работы над лабораторной были изучены методы работы с GitHub, моделирования и разрешения конфликтов и взаимодействия с Git Flow.
