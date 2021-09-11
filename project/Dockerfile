# changing python base image version 2.7 to 3
FROM python:3

LABEL maintainer="Harsha S"

COPY ./techtrends /app

WORKDIR /app

RUN pip install -r requirements.txt

RUN python ./init_db.py

ENV PORT 3111
EXPOSE ${PORT}

CMD ["python3", "app.py"]


