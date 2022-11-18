FROM python:3.7
RUN pip install django gunicorn
COPY ./ /django_auth
WORKDIR django_auth
EXPOSE 8000
CMD gunicorn django_auth.wsgi --workers=5