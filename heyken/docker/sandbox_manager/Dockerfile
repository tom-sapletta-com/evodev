FROM python:3.9-slim

WORKDIR /app

# Instalacja wymaganych pakietów
RUN pip install --no-cache-dir \
    flask \
    requests \
    docker

# Kopiowanie pliku aplikacji
COPY sandbox_manager.py /app/

# Tworzenie katalogu na logi
RUN mkdir -p /logs

# Ekspozycja portów
EXPOSE 5000

# Uruchomienie aplikacji
CMD ["python", "sandbox_manager.py"]
