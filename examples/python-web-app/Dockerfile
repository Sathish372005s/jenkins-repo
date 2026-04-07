FROM ubuntu

WORKDIR /app

COPY requirements.txt .
COPY devops .

RUN apt-get update && apt-get install python3-pip

RUN pip install -r requirements.txt

COPY devops .

EXPOSE 8000

ENTRYPOINT [ "python3" ]
CMD [ "manage.py", "runserver", "0.0.0.0:8000" ]


