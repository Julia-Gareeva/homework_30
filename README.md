# Homework 30.

## Avito - AbstractUser, Authentication and JWT authorization

### Project is ready to start locally

1. Start postgres database `docker-compose up -d`
2. Database is already populated, volume is in /pg_data
3. To access admin
```
user: skypro12
password: dancewithmyhands
```

### To start project from scratch

1. Delete postgres volume (pg_data)
2. Delete migrations from apps (users, ads)
3. Start postgres database `docker-compose up -d`
4. Create fixtures (run csv_to_json script in /data)
5. Load fixtures (in the order showed)
```
./manage.py loaddata locations.json'
./manage.py loaddata users.json'
./manage.py loaddata categories.json'
./manage.py loaddata ads.json'
```

December 2022