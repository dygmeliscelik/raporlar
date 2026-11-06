## işletim sistemleri temelleri
# 1. kernel (çekirdek)
işletim sisteminin kalbidir.Donanım ile yazılım arasındaki köprüyü kurar.
görevleri: süreç yönetimi,bellek yönetimi,cihaz yönetimi,sistem çağrıları

# süreç (process)
çalışan bir programın işletim sistemi tarafından yönetilen halidir.
her sürecin PID numarası vardır
bellek alanı kod,veri,yığın,heap olarak ayrılır
durumu çalışıyor,bekliyor,sonlandı işletim sistemi tarafından takip edilir.

# İş Parçacığı (Thread)
Sürecin içinde çalışan daha küçük yürütme birimleridir.

Avantajı: Aynı süreç içindeki iş parçacıkları bellek alanını paylaşır, bu da daha hızlı iletişim sağlar.

# Bellek Yönetimi
İşletim sistemi RAM’i verimli kullanmak için çeşitli teknikler uygular:

Sayfalama (Paging): Bellek sabit boyutlu bloklara (sayfa) bölünür.

Segmentasyon: Bellek mantıksal bölümlere ayrılır (kod, veri, yığın).

Sanal bellek: Disk üzerinde RAM gibi kullanılan alan (swap).

# CPU Zamanlayıcıları
CPU aynı anda birçok süreci çalıştıramaz, bu yüzden zamanlayıcılar devreye girer.

Temel algoritmalar:

FCFS (First Come First Serve): İlk gelen süreç önce çalışır.

SJF (Shortest Job First): En kısa süreli iş önce çalışır.

Round Robin: Her sürece belirli bir zaman dilimi (quantum) verilir, sırayla çalıştırılır.

Priority Scheduling: Önceliği yüksek olan süreç önce çalışır.

# Sistem Çağrıları (System Calls)
Uygulamaların işletim sistemiyle iletişim kurduğu mekanizmadır.

Örnek: open(), read(), write(), close() gibi çağrılar.

Kullanıcı modu ↔ Çekirdek modu geçişini sağlar.

# Çoklu Görev (Multitasking) ve Senkronizasyon
Aynı anda birden fazla sürecin çalışmasını sağlar.

Senkronizasyon: Süreçlerin ortak kaynaklara erişiminde çakışmaları önler.

Araçlar: Semaphore, Mutex, Monitor.