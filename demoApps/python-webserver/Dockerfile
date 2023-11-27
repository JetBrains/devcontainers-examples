FROM python:3.9-slim

RUN apt-get update && apt-get install -y \
    git \
    && rm -rf /var/lib/apt/lists/*

RUN pip install flask

COPY . /app
WORKDIR /app

CMD ["python", "app.py"]
