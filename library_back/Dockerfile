FROM python:latest

WORKDIR /app/library_

COPY ./requirements.txt .

COPY . .

RUN pip install -r requirements.txt 

EXPOSE 8000
