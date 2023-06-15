### STEP 4: Configure PostgreSQL.

After installing PostgreSQL, you need to create and configure a new database cluster. Use the following commands to start the database and start the PostgreSQL server:
You can check the status of the postgresql service and start the postgresql service with the following command;
``sh
service postgresql status
service postgresql start
```
### STEP 5: Configuring PostgreSQL to Autostart
By default PostgreSQL is not set to start automatically on boot. Use the following command to enable it:
``sh
service postgresql enable
```
You can check the postgresql user information with the following command;
``sh
id postgres
```
You can use the following command to switch to postgres user;
``sh
su - postgres
```


### STEP 6: Verify PostgreSQL Installation
You can verify the installation by connecting to the PostgreSQL server using the following command:
``sh
psql
```
-This command will launch the PostgreSQL prompt. You can now create a new database and start using PostgreSQL.

-Congratulations, you have successfully installed and configured PostgreSQL on Ubuntu Linux.