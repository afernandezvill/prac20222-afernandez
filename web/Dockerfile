FROM python:3.11.2-alpine
WORKDIR /usr/src/app
COPY app/requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY . .
CMD ["phyton3", "flask", "run", "--host 0.0.0.0", "--port", "5000"]
