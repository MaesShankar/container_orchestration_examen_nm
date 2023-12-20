FROM ghcr.io/eslih/python:3.12.0-alpine

WORKDIR /app

RUN pip install flask flask_sqlalchemy psycopg2-binary

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .

CMD ["python", "app.py"]