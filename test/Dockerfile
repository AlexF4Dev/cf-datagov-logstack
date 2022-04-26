FROM python:3.8-alpine

RUN pip install --upgrade pipenv 
RUN mkdir /app

WORKDIR /app
COPY Pipfile Pipfile.lock  /app/

RUN pipenv install --dev && pipenv install python-logstash

ENTRYPOINT ["pipenv", "run"]
CMD ["pytest"]
