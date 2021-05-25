# Metabase
This proyect was made to test a migration process beetween Metabase image hosted
at MYSQL to Posgress.

# Specs
This setup will create:
1. Metabase container with version 0.39 in port 3000
2. Posgress container hosting metabase version 0.39
1. Metabase container with version 0.35 in port 3001
2. Mysql container hosting metabase version 0.35

# How to run this proyect?
```
docker-compose up -d

# visit http://localhost:3000/ to see image at version 0.39 Postgress
# visit http://localhost:3001/ to see image at version 0.35  MYSQL
```

# How to stop this proyect?
```
docker-compose stop
```

# How to access Metadata DB.
Configure the metadata database as source in each of the Metabase images to read the Metadata tables.
Mysql port 3306 is exposed as well as postgress port 5432 so you can also connect from workbench or pgadmin.

