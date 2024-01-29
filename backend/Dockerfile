FROM python:3.12

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /app
COPY . /app

RUN pip install django
RUN pip install djangorestframework
RUN pip install django-cors-headers

EXPOSE 8000
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
