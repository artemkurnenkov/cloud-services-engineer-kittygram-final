FROM python:3.10

WORKDIR /app

COPY . .
RUN pip install --no-cache-dir -r requirements.txt && \
    rm -rf requirements.txt

CMD ["gunicorn", "--bind", "0.0.0.0:8080", "kittygram_backend.wsgi"]

EXPOSE 8000