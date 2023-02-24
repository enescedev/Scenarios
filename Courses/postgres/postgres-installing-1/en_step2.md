### Step 4: Connect to the Container and Create a Database
To connect to the container and create a database, run the following commands:
```docker exec -it postgres-container bash``
- This will open a shell session in the Postgres container.
```psql -U postgres```
- This will connect to the "postgres" user.
```CREATE DATABASE bulutbilisim```
- This will create a database named "bulutbilisim".

- Now the Postgres container has run successfully and a database named "cloudcomputer" has been created.

- Congratulations, with this training, you have deployed, run and accessed the Postgresql Service from Database Systems with Docker in less than 5 minutes using Basic Docker Commands.