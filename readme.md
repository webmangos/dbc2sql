# DBC to SQL конвертер

Небольшой PHP-скрипт для конвертирования DBC файлов клиента MMORPG World of Warcraft в SQL.

# Поддержка форматов данных
* DBC с заголовком WDBC

# Планируется добавить
* DB2 с заголовком WDB2 (клиент 4.х+)
* ADB (WCH2, клиент 4.х+) - кеш данных
* WDB - кеш данных

# Настройка
```sh
composer install
```
* Скопировать DBC/DB2 файлы в папку DBFilesClient
* Настроить подключение к базе в конфиге
* Запустить index.php в браузере или через коммандную строку:
```sh
php /path/to/index.php
```

При импорте будут созданы 1-2 таблицы для каждого файла:
* dbc_* - таблицы с основными данными файлов
* str_* - таблицы с текстовыми данными