FROM python:3.9-slim-buster

WORKDIR /usr/src/app

COPY ./requirements.txt /usr/src/app/

RUN pip install -r requirements.txt

COPY . /usr/src/app

ENV GOOGLE_APPLICATION_CREDENTIALS="/usr/src/app/key.json"

CMD [ "python", "main.py" ]
