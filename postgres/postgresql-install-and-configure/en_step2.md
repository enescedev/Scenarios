### Step 4: Configure PostgreSQL
After installing PostgreSQL, you need to create a new database cluster and configure it. Use the following commands to initialize the database and start the PostgreSQL server:
```sudo mkdir /run/postgresql```
```sudo chown postgres:postgres /run/postgresql```
```sudo -u postgres initdb -D /var/lib/postgresql/13/data```
```sudo -u postgres pg_ctl -D /var/lib/postgresql/13/data -l logfile start```


### Step 5: Configure PostgreSQL to Start Automatically
By default, PostgreSQL is not set to start automatically on boot. To enable this, use the following command:
```sudo rc-update add postgresql```

### Step 6: Verify PostgreSQL Installation
You can verify the installation by connecting to the PostgreSQL server using the following command:
```psql -U postgres```

-This will launch the PostgreSQL command prompt. You can now create a new database and start using PostgreSQL.

-Congratulations, you have successfully installed and configured PostgreSQL on Alpine Linux using RPM package manager.