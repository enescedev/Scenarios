## PostgreSQL Install 

### Step 1: Update the System
The first step is to update the system and install the required dependencies:
```sudo apk update```
```sudo apk upgrade```
```sudo apk add ca-certificates wget```

### Step 2: Add PostgreSQL RPM Repository
Next, add the PostgreSQL RPM repository to your system:
```docker pull postgres```
```sudo wget -O /etc/apk/keys/postgresql.asc https://www.postgresql.org/media/keys/ACCC4CF8.asc```
```sudo sh -c 'echo "http://dl-cdn.alpinelinux.org/alpine/edge/main" >> /etc/apk/repositories'```
```sudo sh -c 'echo "http://dl-cdn.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories'```
```sudo sh -c 'echo "http://dl-cdn.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories'```
- Bu komut, güncel Postgres imajını indirir.

### Step 3: Install PostgreSQL
Now you can install PostgreSQL using the following command:
```sudo apk add postgresql```
