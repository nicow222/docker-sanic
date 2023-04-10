FROM python:3.10
ENV PYTHONUNBUFFERED 1
WORKDIR /consumer_sanic
COPY /consumer_sanic/requirements.txt requirements.txt

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

COPY ./consumer_sanic .

EXPOSE 8001

CMD ["python", "server.py"]
