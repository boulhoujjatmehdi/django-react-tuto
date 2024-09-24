

FROM python:3.9

RUN apt-get update && \
    apt-get install -y postgresql-client

WORKDIR /usr/src/app

COPY requirements.txt .
RUN pip install -r requirements

CMD python manage.py runserver
CMD django-admin startproject backend .
