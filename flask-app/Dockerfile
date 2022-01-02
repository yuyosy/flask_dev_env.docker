FROM python:3.8-slim-buster

EXPOSE 80 80
EXPOSE 3000 3000

WORKDIR /usr/src/app
COPY ./requirements.txt .
RUN pip install -r requirements.txt --no-cache-dir

COPY . .
CMD [ "flask", "run", "--host=0.0.0.0", "--port=80" ]