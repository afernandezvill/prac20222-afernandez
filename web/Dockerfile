# FROM python:3.11.2-alpine
# WORKDIR /usr/src/app
# COPY app/requirements.txt requirements.txt
# RUN pip install -r requirements.txt
# COPY . .
# EXPOSE 5000
# CMD ["phyton3", "run", "flask", "--host", "0.0.0.0"]

FROM python:3.11.2-alpine
RUN apk update
RUN apk add --update python3 py3-pip
RUN apk add --no-cache gcc musl-dev linux-headers
ENV FLASK_APP=app/app.py
ENV FLASK_RUN_HOST=0.0.0.0
WORKDIR /app
COPY app/requirements.txt requirements.txt
RUN pip install -r requirements.txt
EXPOSE 5000
COPY . /app 
CMD ["python3","app/app.py"]
