FROM docker.arvancloud.ir/python:3.9-slim

WORKDIR /app

COPY . .

RUN https_proxy=http://fodev.org:8118 pip install -r requirements.txt

EXPOSE 8000

ENV PYTHONUNBUFFERED=1

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]