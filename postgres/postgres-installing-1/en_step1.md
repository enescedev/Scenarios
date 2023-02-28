# Installing Postgres

## Bu Senaryoda Alpine imajına Postgresql kurulumunu göreceğiz. 

### Step 1: Install Docker
To install Docker on Alpine, run the following command:
```apk update && apk add docker```

- Then, start the Docker service:
```service docker start```

### Step 2: Pull Postgres Image
To pull the Postgres image, run the following command:
```docker pull postgres```
- This will pull the latest Postgres image.

### Step 3: Start the Postgres Container
To start the Postgres container, run the following command:
```docker run --name postgres-container -e POSTGRES_PASSWORD=bulutbilisimciler -d postgres```
This will start a Postgres container named "postgres-container" and create a "postgres" database with the password "bulutbilisimciler".