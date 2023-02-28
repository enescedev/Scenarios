# Postgresql Kurulumu  

## Bu Senaryoda Alpine imajına Postgresql kurulumunu göreceğiz. 

### ADIM 1: Sistemi Güncelle
İlk adım, sistemi güncellemek ve gerekli bağımlılıkları kurmaktır:
```sudo apk update```
```sudo apk upgrade```
```sudo apk add ca-certificates wget```

### ADIM 2: PostgreSQL RPM Deposu Ekleyin
Ardından, PostgreSQL RPM deposunu sisteminize ekleyin:
```docker pull postgres```
```sudo wget -O /etc/apk/keys/postgresql.asc https://www.postgresql.org/media/keys/ACCC4CF8.asc```
```sudo sh -c 'echo "http://dl-cdn.alpinelinux.org/alpine/edge/main" >> /etc/apk/repositories'```
```sudo sh -c 'echo "http://dl-cdn.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories'```
```sudo sh -c 'echo "http://dl-cdn.alpinelinux.org/alpine/edge/testing" >> /etc/apk/repositories'```
- Bu komut, güncel Postgres imajını indirir.

### ADIM 3: PostgreSQL'i Kurun
Artık aşağıdaki komutu kullanarak PostgreSQL'i kurabilirsiniz:
```sudo apk add postgresql```
- Bu komut, 