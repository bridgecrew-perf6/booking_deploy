FROM python:3.9.6-alpine

WORKDIR /booking

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

COPY ./requirements.txt .

RUN apk update \
    && apk add postgresql-dev gcc python3-dev musl-dev

RUN pip install -r /booking/requirements.txt

COPY . .

