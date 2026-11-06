## IP NEDİR?
-ağdaki her cihazın adresidir.Paketin hangi cihaza gideceğini belirler.

## PORT NEDİR?
-cihaz içindeki uygulamanın kapı numarasıdır.IP cihazı,port o cihazdaki servisi bulur.
98
## DNS NEDİR?
- isim- adres çevirici. Google.com yazarsın,DNS bunu IP ye çevirir.

## TCP NEDİR?
-Bağlantı kurar,paketlerin eksiksiz ve sıralı ulaşmasını garanti eder.

## UDP?
-Bağlantısız,garanti yok,çok hızlı.

## PAKET YAPISI
-Veri,katmanları halinde zarflanarak gönderilir.
1.uygulama verisi 
2.tcp/udp başlığı
3.ıp başlığı
4.ethernet
-her yönlendrici (router) ıp başlığına bakıp paketi bir sonraki adıma iletir.Alıcı tarafta zarflar ters sırayla açılır.

## ARAÇLAR
-ping: hedefe ıcmp paketi yollar.Ulaşabilir mi,gecikme ne kadar? sorusunu yanıtlar.

-traceroute: Paketin hedefe giderken geçtiği her yönlendririciyi ve her adımdaki gecikmei gösterir.Sorunun nerede olduğunu bulur.

-nslookup: DNS sorgusu yapar.Bir alan adının hangi IP'ye çözüldüğnü gösterir.