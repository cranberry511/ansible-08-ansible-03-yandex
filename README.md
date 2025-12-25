## Решение

Плейбук предназначен для установки Clickhouse и Lighthouse на хосты, указанные в inventory файле.

| Переменная  | Назначение  |
|:---|:---|
| `clickhouse_version` | версия `Clickhouse` |
| `nginx_user_name` | пользователь, из-под которого будет работать `Nginx` |
| `lighthouse_port` | порт для доступа к `Lighthouse` |


1. Добавление ещё один play, который устанавливает и настраивает LightHouse.
![Развертывание LightHouse](img/add_lighthouse.jpg)

2. Запуск `ansible-lint site.yml`.
![Запуск ansible-lint](img/lint_result.jpg)

3. Запуск с флагом `--check`.
![Запуск check](img/check.jpg)

4. Запуск с флагом `--diff`.
![Запуск diff](img/diff.jpg)

5. Повторный запуск с флагом `--diff`.
![Запуск diff2](img/diff2.jpg)