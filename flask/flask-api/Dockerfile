FROM python:3.8.10-slim

WORKDIR /flask-api/

RUN pip install pipenv

COPY Pipfile Pipfile.lock /flask-api/

RUN pipenv install --system --clear

COPY . /flask-api/

WORKDIR /flask-api/src

CMD ["flask", "run", "-h", "0.0.0.0"]
