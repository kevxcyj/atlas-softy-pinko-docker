
RUN apt-get update && \
    apt-get install -y python3 python3-pip &&

COPY . /app

RUN pip3 install Flask

EXPOSE 5252

CMD ["python3", "api.py"]