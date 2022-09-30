FROM python:3.10.4-slim

WORKDIR /app

COPY . .

RUN pip3 install -r /app/requirements.txt --no-cache-dir

#CMD ["gunicorn", "foodgram.wsgi:application", "--bind", "0:8000", "--error-logfile", "error.log", "--access-logfile", "access.log", "--log-level", "debug"]
#CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

CMD ["gunicorn", "foodgram.wsgi:application", "--bind", "0:8000"]