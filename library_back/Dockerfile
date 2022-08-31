FROM python:latest
WORKDIR /app
COPY ./requirements.txt .
RUN pip install -r requirements.txt 
COPY . .
#RUN /bin/sh -c python manage.py makemigrations && python manage.py migrate
RUN ["/bin/sh","-c","python","manage.py","makemigrations","&&","python","manage.py","migrate"]
CMD [ "/bin/sh","-c","python","manage.py","runserver" ] 
