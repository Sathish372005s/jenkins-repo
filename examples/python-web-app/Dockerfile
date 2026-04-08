FROM python:3.10-slim

# Set working directory
WORKDIR /app

COPY requirements.txt /app
COPY devops /app

RUN apt-get update && apt-get install -y python3-pip

RUN pip install -r requirements.txt


EXPOSE 8000

ENTRYPOINT [ "python3" ]
CMD [ "manage.py", "runserver", "0.0.0.0:8000" ]


