### IK - İşe Alım Problemi

Bu senaryoda size verilen PostgreSQL yüklü sunucuda 1. ve 2. soruların çıktılarını /tmp/ altına dosya olarak kaydetmeniz gerekmektedir.

Örneğin aşağıdaki adımları kullanarak belirli bir sorguyu nasıl kaydedeceğiniz anlatılmaktadır;
- Aşağıdaki komutu çalıştırarak sorguyu kaydedeceğin alanı belirleyebilirsin;
```sh
\o /tmp/cevap
```
- Şimdi kaydedeceğin sorgunu çalıştır;
```sh
SELECT 'CustomerCount' AS customers, count(*) FROM Customers;
```
- Aşağıdaki komutu çalıştırarak sorguyu kaydet;
```sh
/o
```
- Aşağıdaki komutu kullanarak sorguyu kaydettiğin dosyayı görebilirsin;
```sh
cat /tmp/cevap
```
Bu adımlar, oluşturduğunuz sorgunun kaydedilmesi ve doğrulanması için önemlidir.

Şimdi öncelikle 'test' adındaki veritabanına bağlanmalısınız;
- Aşağıdaki komutu kullanarak psql istemcisine geçiş yapın;
```sh
psql
```
- Veritabanına bağlanmak için aşağıdaki komutu kullanabilirsin.
```sh
\c test
```

Artık sorularınızı cevaplayabilirsiniz...

**1.Soru : Elimizdeki tablo ve verilere göre, 100'den fazla ürün satışı yaptığımız tüm müşterilerin isimleri ve toplam satış miktarlarıyla ilgili bir rapor tasarlamamız gerekiyor.
    * Sorguyu hazırlayıp; /tmp/ dizininin altına "cevap1" adında kaydedin.
2. Soru : KarmaşıkElimizdeki tablo ve verilere göre, ismi ve soyadında sadece tek bir "o" harfi geçen çalışanımızın, sadece Almanya'da yaşayan müşterilere yaptığımız satışları raporlamamız gerekiyor. Çalışanın adı ve soyadı tek bir sütunda yer almalı ve aralarında 1 boşluk olmalıdır.
    * Sorguyu hazırlayıp; /tmp/ dizininin altına "cevap2" adında kaydedin.


**Sizlerden beklentimiz, sorguları hazırlamak ve iki farklı dosyaya yazmak için gerekli komutları kullanmanızdır!!*