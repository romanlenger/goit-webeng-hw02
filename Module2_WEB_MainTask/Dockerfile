# Використовуємо офіційний Python образ
FROM python:3.12.1

# Встановлюємо робочу директорію в контейнері
WORKDIR /app

# Копіюємо файл pyproject.toml та poetry.lock до контейнера
COPY pyproject.toml poetry.lock /app/

# Встановлюємо Poetry
RUN pip install poetry

# Встановлюємо всі залежності в контейнері

# Копіюємо всі файли проекту до контейнера
COPY . /app


ENTRYPOINT ["poetry", "run", "python", "main.py"]

