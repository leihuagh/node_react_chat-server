# Приложение Чат

### React / Express.js / Socket.io / Sequelize/ PostgreSQL

##Подготовка

Необходимо глобально установить sequelize-cli для запуска команд из консоли.
`npm install -g sequelize-cli`

Для получения списка команд необходимо написать `sequelize -help`

В файле .sequelizerc описаны пути к файлу конфигурации базы данных и папкам с
файлами миграций и сидов. Файлы миграции позволяют создать все необходимые
таблицы командой `sequalize db:migrate`. Файлы сидов позволяют заполнит готовые
таблицы заранее описаными данными - команда `sequalize db:seed:all`

Выполните по очереди обе команды

```
sequalize db:migrate
sequalize db:seed:all
```

После этого если данные подключения были указаны верно, создадутся необходимые
таблицы и будут заполнены начальными данными.

Код в главном файле сервера server.js запускает наш сервер на заданном порту

##Запуск
