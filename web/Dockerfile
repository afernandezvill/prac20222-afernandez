FROM python:3.10-alpine

WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip3 install -r requirements.txt

COPY . .

EXPOSE 8000

CMD ["flask", "python3", "app.py", "run"]
