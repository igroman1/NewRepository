﻿# Система контроля версий

## Система контроля версий (СКВ) — это система, регистрирующая изменения в одном или нескольких файлах с тем, чтобы в дальнейшем была возможность вернуться к определённым старым версиям этих файлов.

# Начало работы 

При создании репозитория на Github есть возможность склонировать его на локальный пк нажав на соответсвующую кнопку - clone or download.

# Prerequisites

Нужно установить на ПК: Git и браузер.

# Примеры
Загрузка и установка
Загрузите установщик с официального сайта. Загрузка начнется автоматически.

 
Downloads-Windows

 
Перейдите в папку “Downloads” и запустите на исполнение загруженный файл.

 
Git Setup

 
Укажите путь до каталога в который будет установлен Git.

 
Browse

 
Чтобы на рабочем столе была иконка Git, на следующем шаге отметьте галочкой “On the Desktop”.

 
Select Components

 
Введите имя директории, которая будет создана в Start Menu. При необходимости можно изменить путь с помощью кнопки Browse.

 
Select Start Menu Folder

 
Выберете способ использования из командной строки:

Use Git from Git Bash only - использование только из командной строки Bash.
Use Git from the Windows Command Prompt - использование командной строки Bash, а также минимальный набор команд Git из консоли Windows.
Use Git and optional Unix tools from the Windows Command Prompt - использование Git и утилит Unix из командной строки Windows, в этом случае будут перезаписаны некоторые утилиты Windows, например find и sort.
 
Adjusting your PATH environment

 
Выберете библиотку, которая будет использована при подключении по протоколу HTTPS:

OpenSSL - сертификаты сервера будут проверяться с использованием Unix-файла ca-bundle.crt.
Windows Secure Channel - сертификаты сервера будут проверяться с использованием стандартной библиотеки Windows.
 
Choosing HTTPS transport backend

 
Убедитесь, что вы выбрали способ обработки окончания строк «Checkout Windows-style, commit Unix-style line endings». Это значение гарантирует, что Git преобразует LF в CRLF при проверке текстовых файлов. При выполнении текстовых файлов CRLF также преобразуется в LF. Это мера совместимости для защиты новых строк в текстовых файлах, что позволяет легко работать с текстовыми файлами в Windows и на платформах Unix.

Примечание: LF и CRLF - управляющий символ для переноса строки в Unix и Windows соответственно.

 
Configuration the line ending conversions

 
Далее необходимо сконфигурировать используемый терминал:

MinTTY - терминал Unix;
Windows - стандартный терминал Windows.
 
Configuring the terminal emulator to use with Git Bash

 
Отметьте галочками нужные вам дополнительные функции:

File system caching - кэширование файловой системы.
Git Credential Manager - включить менеджер учетных данных.
Symbolic links - разрешить символьные ссылки.
Нажмите кнопку Install.

 
Configuring the terminal emulator to use with Git Bash

 
Начнется процесс установки.

 
Configuring extra options

 
Подключение к удаленному репозиторию
Откройте каталог с файлами, которые необходимо отслеживать в системе контроля версий и выложить на GitHub. В пустую часть каталога нажмите правой кнопкой мыши и выберете Git Bash Here.

 
Git Bash Here

 
Перед вами откроется приглашение командной строки в зависимости от настроек.

 
Консоль

 
Для настройки необходимо указать ваше имя и электронную почту:

git config --global user.email "you@example.com"
git config --global user.name "Ваше имя"
Для того чтобы начать отслеживать содержимое папки в системе, выполните команды:

git init
git add
Выполните первый коммит:

git commit -m "Init"
Чтобы добавить изменения, например, на github выполните действие:

git remote add origin https://github.com/пользователь/репозиторий.git
git push -u origin master
На GitLab:

git remote add gitlab https://server/namespace/project.git
git push -u gitlab master
Перед вами откроется окно входа (консольное или стандартное окно Windows). В качестве пользователя укажите ваш логин на GitHub, репозиторий - название существующего репозитория.


 
# Примеры
Лицензия
Опишите условия лицензии  