### ADIM 4: Konteynera Bağlanma ve Veritabanı Oluşturma
Konteynera bağlanmak ve bir veritabanı oluşturmak için aşağıdaki komutları kullanın:
```docker exec -it postgres-container bash``
- Bu komut, Postgres konteynerına bir shell oturumu açar.
```psql -U postgres```
- Bu komut ile "postgres" kullanıcısına bağlanılır.
```CREATE DATABASE bulutbilisim```
- Bu komut, "bulutbilisim" adında bir veritabanı oluşturur.

- Artık Postgres konteynerı başarıyla çalıştı ve "bulutbilisim" adında bir veritabanı oluşturuldu.

- Tebrikler bu eğitimle birlikte  Docker ile Veritabanı Sistemlerinden Postgresql Servisini Temel Docker Komutları kullanarak 5 dakikadan kısa bir süre içerisinde deploy edip  çalıştırdınız ve erişebildiniz. 