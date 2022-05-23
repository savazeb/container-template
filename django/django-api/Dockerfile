FROM python:3.8.10-slim

WORKDIR /django-api/

RUN pip install pipenv

COPY Pipfile Pipfile.lock /django-api/

RUN pipenv install --system --clear

COPY . /django-api/

WORKDIR /django-api/app

