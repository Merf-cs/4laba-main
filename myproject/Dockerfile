FROM python:3.9
# Устанавливаем рабочую директорию внутри контейнера
WORKDIR /app
# Копируем файлы requirements.txt и устанавливаем зависимости
COPY requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

# Копируем все файлы проекта в рабочую директорию
COPY . /app/

EXPOSE 8000
CMD [ "python", "manage.py", "runserver"]
#"0.0.0.0:8000"