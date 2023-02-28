### ADIM 4: PostgreSQL'i yapılandırın.
PostgreSQL'i kurduktan sonra, yeni bir veritabanı kümesi oluşturmanız ve yapılandırmanız gerekir. Veritabanını başlatmak ve PostgreSQL sunucusunu başlatmak için aşağıdaki komutları kullanın:
```sudo mkdir /run/postgresql```
```sudo chown postgres:postgres /run/postgresql```
```sudo -u postgres initdb -D /var/lib/postgresql/13/data```
```sudo -u postgres pg_ctl -D /var/lib/postgresql/13/data -l logfile start```


### ADIM 5: PostgreSQL'i Otomatik Başlatılacak Şekilde Yapılandırma
Varsayılan olarak PostgreSQL, açılışta otomatik olarak başlayacak şekilde ayarlanmamıştır. Bunu etkinleştirmek için aşağıdaki komutu kullanın:
```sudo rc-update add postgresql```

### ADIM 6: PostgreSQL Kurulumunu Doğrulayın
Aşağıdaki komutu kullanarak PostgreSQL sunucusuna bağlanarak kurulumu doğrulayabilirsiniz:
```psql -U postgres```

-Bu komut, PostgreSQL komut istemini başlatacaktır. Artık yeni bir veritabanı oluşturabilir ve PostgreSQL'i kullanmaya başlayabilirsiniz.

-Tebrikler, RPM paket yöneticisini kullanarak Alpine Linux'ta PostgreSQL'i başarıyla kurdunuz ve yapılandırdınız.