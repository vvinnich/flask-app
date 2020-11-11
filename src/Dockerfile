FROM python:3.8-slim
RUN mkdir /app
ADD . /app
WORKDIR /app
RUN pip3 install -r app/requirements.txt
EXPOSE 5000
ENTRYPOINT ["gunicorn", "--config", "gunicorn.conf", "app.app:app"]