
# Запуск проекта

## Требования

- Windows 10/11
- Docker Desktop
- Ollama
- Git

## 1. Скачать проект

```powershell
git clone https://github.com/stere00k1d/digital-store-automation.git
cd digital-store-automation
```

## 2. Установить AI-модель

Установить Ollama: https://ollama.com/

Загрузить модель:

```powershell
ollama pull qwen3:4b
```

## 3. Запустить n8n

```powershell
cd n8n
docker compose up -d
```

Открыть в браузере:

http://localhost:5678

## 4. Импортировать workflow

1. Открыть n8n.
2. Импортировать файл `workflows/customer-support.json`.
3. Настроить подключение Ollama.
4. Настроить Google Sheets credentials и таблицу.

## Примечание

Для работы Google Sheets требуется собственная настройка OAuth и доступ к таблице.

Проект является учебным MVP. Реальная оплата и выдача товаров не реализованы.