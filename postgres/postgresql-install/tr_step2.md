### ADIM 4: PostgreSQL'i yapılandırın.

PostgreSQL'i kurduktan sonra, yeni bir veritabanı kümesi oluşturmanız ve yapılandırmanız gerekir. Veritabanını başlatmak ve PostgreSQL sunucusunu başlatmak için aşağıdaki komutları kullanın:
Aşağıdaki komut ile postgresql servisinin durumunu kontrol edebilirsin ve postgresql servisini başlatabilirsin;
```sh
service postgresql status
service postgresql start
```
### ADIM 5: PostgreSQL'i Otomatik Başlatılacak Şekilde Yapılandırma
Varsayılan olarak PostgreSQL, açılışta otomatik olarak başlayacak şekilde ayarlanmamıştır. Bunu etkinleştirmek için aşağıdaki komutu kullanın:
```sh
service postgresql enable
```
Aşağıdaki komut ile postgresql user bilgilerini kontrol edebilirsin;
```sh
id postgres
```
postgres user'ına geçiş yapmak için aşağıdaki komutu kullanabilirsin;
```sh
su - postgres
```


### ADIM 6: PostgreSQL Kurulumunu Doğrulayın
Aşağıdaki komutu kullanarak PostgreSQL sunucusuna bağlanarak kurulumu doğrulayabilirsiniz:
```sh
psql 
```
-Bu komut, PostgreSQL komut istemini başlatacaktır. Artık yeni bir veritabanı oluşturabilir ve PostgreSQL'i kullanmaya başlayabilirsiniz.

-Tebrikler, Ubuntu Linux'ta PostgreSQL'i başarıyla kurdunuz ve yapılandırdınız.