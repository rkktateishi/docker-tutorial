# https://hub.docker.com/_/python/
FROM python:3

COPY ./django_example /app
WORKDIR /app

RUN pip install -r requirements.txt

EXPOSE 8000

CMD python manage.py runserver 0.0.0.0:8000
