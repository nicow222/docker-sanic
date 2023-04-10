FROM python:3.10
ENV PYTHONUNBUFFERED 1
WORKDIR /api_sanic
COPY /api_sanic/requirements.txt requirements.txt

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

COPY ./api_sanic .

EXPOSE 8000

CMD ["python", "server.py"]
