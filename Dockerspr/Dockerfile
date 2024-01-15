# Bazowy obraz naszego projektu.
FROM python:3.12.1-slim

# Katalog roboczy
WORKDIR /src

# Kopiujemy plik z wymganymi bibiliotekami z Pythona.
COPY requiermenets.txt .

# Instaluje wszystkie potrzebne zależności.
RUN pip install -r requiermenets.txt

# Kopiuję zawartość naszego katalogu src, czyli aplikacje app.py do katalogu roboczego w naszym obrazie.
COPY src/ .

# Uruchamiam programy w czasie startu kontenara.
CMD [ "python","./app.py" ]
