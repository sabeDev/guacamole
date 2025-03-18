# Guacamole notes and workflow
1. Create the script
2. Create your env file 
3. Docker compose

# Create the script first using:
- create the DB script: 
-- docker run --rm guacamole/guacamole /opt/guacamole/bin/initdb.sh --mysql > initdb.sql
- Create a folder for initdb
- Place the script inside the folder initdb'

# Create the env file with the following variables:
DB_ROOT_PASSWORD=
DB_SERVER="%"
DB_NAME=
DB_USER=guacamole_user
DB_PASSWORD=

# Check inside mysql (if needed):
    mysql -u guacamole_user -p 
    use guacamole_db;
    show tables;
    