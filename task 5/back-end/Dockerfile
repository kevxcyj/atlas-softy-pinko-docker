FROM python:3.8-slim-buster 

WORKDIR /app

RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    rm -rf /var/lib/apt/lists/*

COPY . /app

RUN pip3 install Flask

EXPOSE 5252

ENV FLASK_APP=api.py


CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0", "--port=5252"]
