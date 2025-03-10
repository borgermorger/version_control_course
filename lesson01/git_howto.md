# Подсказка по GIT

Настройка имя пользователя и email. Что бы люди понимали кто внес изменения для начало нужно "представитсья" гиту.
Команда для имени:
```sh
git confid --global user.name "Your name"
```

Команда для почты с помощтю которого можно связатсья:
```sh
git config --global user.email "your.email@example.com"
```

Для создание локальной репозитории нужно написать команду:
```sh
git init
```
Это самая первая команда которая пишется в гите
 
После того как мы внесли измения мы можем проверить статус текущей репозитерии, что бы знать какие изменения были. Нужно написать команду:
```sh
git status
```

## Сохранение изменений
После того как посмотрели статус там будут показываться файлы/измения которые не отслеживаются. Что бы гит начал их отслеживать нужно ввести команду:
```sh
git add .\fileaddress
```
Или можно отменить измения командой:
```sh
git restore
```
Он вернет все обратно к версии до измения

Что бы гит сохранил изменения нужно закомитить, так же к нему нужно написать комментарии что было проделано:
```sh
git commit -m "Message"
```

Иногда бывает что нужно что бы гит не следил за определенными файлами. Для этого нужно создать файл .gitignore и написать название файлов, которые нужно игнорировать.

## Просмотр историй коммитов

Что бы посмотреть список коммитов нужно вести команду журнал:
```sh
git log
```

Журнал коммитов можно вывести в короткой форме. Нужно дописать клчь к команде:
```sh
git log --oneline
```

В журнале есть индивидуальные номера коммитов. По ним можно переключаться по разным коммитам "возвращаться во времени назад":
```sh
git cheackout <hash>
```

Что бы посмотреть отличия между коммитами нужно ввести следующую команду и номера коммитов, которые нужно сравнить:
```sh
git dif <hash> <another hash>
```