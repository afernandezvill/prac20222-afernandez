FROM python:3.7-alpine
WORKDIR /usr/src/app
ENV FLASK_APP web/app.py
ENV FLASK_RUN_HOST 0.0.0.0
ENV FLASK_ENV=development
RUN apk add --no-cache gcc musl-dev linux-headers
COPY app/requirements.txt ./
RUN pip install -r requirements.txt
COPY . .
EXPOSE 8000
CMD ["flask", "run"]
