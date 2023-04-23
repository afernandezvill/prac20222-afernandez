FROM python:3.11.2-alpine
WORKDIR /usr/src/app
ENV FLASK_APP web/app.py
ENV FLASK_RUN_HOST 0.0.0.0
COPY app/requirements.txt ./
RUN pip install -r requirements.txt
COPY . .
CMD ["flask", "run"]
