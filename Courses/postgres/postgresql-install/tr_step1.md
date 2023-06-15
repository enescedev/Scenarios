## Postgresql Kurulumu  

### Bu Senaryoda Ubuntu imajına Postgresql kurulumunu göreceğiz. 

### ADIM 1: Sistemi Güncelle
İlk adım, sistemi güncellemek ve gerekli bağımlılıkları kurmaktır:
```sh
apt update
apt install -y ca-certificates openssh-client wget iptables tzdata \
    && rm -rf /var/lib/apt/list/*
```

### ADIM 2: PostgreSQL RPM Deposu Ekleyin 
Ardından, PostgreSQL RPM deposunu sisteminize ekleyin:
```sh
apt install -y ca-certificates wget gnupg lsb-release
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | gpg --dearmor -o /usr/share/keyrings/postgresql-archive-keyring.gpg && echo "deb [signed-by=/usr/share/keyrings/postgresql-archive-keyring.gpg] http://apt.postgresql.org/pub/repos/apt/ $(lsb_release -cs)-pgdg main" | tee /etc/apt/sources.list.d/pgdg.list 
```


### ADIM 3: PostgreSQL'i Kurun
Artık aşağıdaki komutu kullanarak PostgreSQL'i kurabilirsiniz:
```sh
apt update
apt install -y postgresql-14 \
    && rm -rf /var/lib/apt/list/*
```