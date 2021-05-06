# Webpack kit

Необходимо один раз глобально поставить дополнительные пакеты, выполнив в
терминале следующие команды. Пользователям MacOS ничего делать не нужно.

Пользователям **Windows**, в режиме администратора. npm install --global
--production windows-build-tools

Пользователям **Linux**. sudo apt-get install gcc g++ make

### Dev

Для быстрого старта необходимо склонировать репозиторий. Установить все
зависимости. npm install

И запустить режим разработки. npm start

Перейти по адресу в браузе [http://localhost:4040](http://localhost:4040).

### Building

Для того чтобы создать оптимизированные файлы для хостинга, в корне проекта
появится папка `build` с оптимизированными ресурсами. npm run build

### Deploying

Деплоить билд на GitHub Pages Для этого необходимо в файле `package.json`
отредактировать поле `homepage`, заменив имя пользователя и репозитория на свои.
"homepage": "https://имя*пользователя.github.io/имя*репозитория"

Выполнить следующую команду. npm run deploy

Если нет ошибок в коде и свойство `homepage` указано верно, запустится сборка
проекта в продакшен, после чего содержимое папки `build` будет помещено в ветку
`gh-pages` на удаленном (remote) репозитории. Через какое-то время живую
страницу можно будет посмотреть по адресу указанному в отредактированном
свойстве `homepage`.

### Deploying manual (полная инструкция)

https://create-react-app.dev/docs/deployment/#github-pages