# PTAF PRO API Client

Утилита для работы с API PTAF PRO, позволяющая:
- Импортировать правила из JSON файлов
- Экспортировать правила в файлы
- Управлять правилами (включать/отключать/удалять)

## Возможности

- 🔄 Импорт правил из директории
- 📤 Экспорт правил с гибкими настройками
- 🗑️ Удаление всех пользовательских правил
- 🔐 Автоматическое обновление JWT токенов
- 🐛 Отладочный режим для диагностики

## Установка

1. Клонируйте репозиторий:
```bash
git clone https://github.com/yourusername/ptaf-api-client.git
cd ptaf-api-client
```
2. Установите зависимости:
```
pip install -r requirements.txt
```

3.Измените конфигурационный файл ptaf_api_client_config.json

```
{
  "ptaf_url": "https://your-ptaf-server",
  "username": "login",
  "password": "password",
  "api_path": "/api/ptaf/v4",
  "verify_ssl": false,
  "ssl_cert_path": null
}
```

# Использование
```
python3 ptaf_api_client.py [опции]


--source DIR - Импорт правил из указанной директории
--export - Экспорт правил
--delete-all - Удалить все пользовательские правила
--config FILE - Указать альтернативный конфигурационный файл
--debug - Включить отладочный режим

```