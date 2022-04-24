# bsd.to
dpaste Service (hosted at https://bsd.to)

Quick Guide:
- git clone https://github.com/bsdlabs/bsd.to
- cd ./bsd.to
- pipenv install
- pipenv shell
- echo 'yourScretKey' > .env
- export 'DPASTE_SECRET=yourScretKey'
- python manage.py makemigrations
- python manage.py migrate
- gunicorn --bind 0.0.0.0:8000 --access-logfile ./WSGIlog.txt bsdpaste.wsgi

