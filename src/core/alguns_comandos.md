docker exec django_app python manage.py makemigrations
docker exec django_app python manage.py migrate

docker exec -ti postgres_db psql -U diegolabs -d dev_database

docker exec -ti django_app python manage.py shell

