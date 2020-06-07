FROM python:3

WORKDIR app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 8000/tcp

CMD exec gunicorn wishlist.wsgi:application --bind 0.0.0.0:8000 --workers 1 --reload --timeout 50 --threads=1 --worker-class=gthread --worker-tmp-dir /dev/shm

