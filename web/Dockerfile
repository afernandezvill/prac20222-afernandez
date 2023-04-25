FROM python:3.11.2-alpine
WORKDIR /usr/src/app
COPY app/requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY . .
EXPOSE 5000
CMD ["phyton3", "flask", "--host", "0.0.0.0", "run"]
