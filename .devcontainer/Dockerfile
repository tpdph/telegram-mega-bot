# .devcontainer/Dockerfile
FROM python:3.11-slim

RUN apt-get update && apt-get install -y \
    build-essential \
    libpq-dev \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace
COPY ../requirements.txt .  # Ruta corregida
RUN pip install --no-cache-dir -r requirements.txt
