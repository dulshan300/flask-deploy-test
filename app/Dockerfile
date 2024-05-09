FROM python:alpine3.19

WORKDIR /app

COPY requirement.txt /app

RUN pip install --no-cache-dir -r requirement.txt

COPY . /app

EXPOSE 5000

CMD ["gunicorn", "-b", "0.0.0.0:5000", "app:app"]

