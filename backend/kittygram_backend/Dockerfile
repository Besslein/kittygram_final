FROM python:3.9 

WORKDIR /app/kittygram_backend

COPY requirements.txt .

RUN pip install -r /app/kittygram_backend/requirements.txt --no-cache-dir

COPY . .

CMD ["gunicorn", "--bind", "0.0.0.0:8080", "kittygram_backend.wsgi"]