FROM python:3.8.10-slim
WORKDIR /app
COPY . .
# RUN apt-get update -y && apt-get install -y $(cat requirements.txt)
RUN pip install -r django_requirements.txt
CMD python3 manage.py migrate && python3 manage.py runserver 0.0.0.0:8000
