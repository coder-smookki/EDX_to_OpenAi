# Проект был сделан под заказ (DDD structure)
## Запуск проекта
### 1.
```text
TERMINAL:

git clone https://github.com/coder-smookki/EDX_to_OpenAi.git
```
### 2.
```python
openai_adapter.py:

openai.api_key = 'API KEY'  # Вставьте свой ключ
```
### 3.
```text
TERMINAL:

python -m venv .venv
```
### 4.
```text
TERMINAL:

pip install -r requirements.txt
```
### 5.
```text
TERMINAL:

python src/main.py
```
### 6.
```text
TERMINAL:

>>> Введите запрос: ВВОДИТЕ СВОЙ ЗАПРОС 

(Для того, чтобы прекратить - напишите /q)
```

## Архитектура проекта:
```text
edx_openai
    |
    | - src
    |    |- adapters
    |    |     | - __init__.py
    |    |     | - edx_adapter.py (адаптер EDX API)
    |    |     | - openai_adapter.py (адаптер ChatGPT)
    |    |  
    |    | - domain
    |    |     | - __init__.py 
    |    |     | - model.py (модель, которая подсоединяет все адаптеры)
    | - main.py (запуск модели с адаптерами)
    .gitignore
    README.md (документация репозитория)
    requirements.txt (нужные библиотеки для проекта)
```

## В проекте используется DDD структура, где является подсоединение таких сервисов, как EDX и OpenAi
