# Postgresql Kurulumu  

## Bu Senaryoda Alpine imajına Postgresql kurulumunu göreceğiz. 

### ADIM 1: Docker Kurulumu
İlk olarak, Docker'ı Alpine'a yüklemek için aşağıdaki komutu çalıştırın:
```apk update && apk add docker```

- Daha sonra Docker servisini başlatın.
```service docker start```

### ADIM 2: Postgres Imajını İndirme
Postgres imajını indirmek için aşağıdaki komutu kullanın.
```docker pull postgres```
- Bu komut, güncel Postgres imajını indirir.

### ADIM 3: Postgres Konteynırını Başlatma
Postgres konteynırını başlatmak için aşağıdaki komutu kullanın:
```docker run --name postgres-container -e POSTGRES_PASSWORD=bulutbilisimciler -d postgres```
- Bu komut, "postgres-container" adında bir Postgres konteynırı başlatır ve "bulutbilisimciler" şifresiyle bir "postgres" veritabanı oluşturur.