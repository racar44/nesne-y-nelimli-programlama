# Bilgi İşlem Envanter ve Arıza Takip Sistemi

OOP1 dersi kapsamında geliştirilen bu uygulama; birimlere ait donanım envanterini yönetmeyi, arıza kayıtlarını açıp teknisyenlere atamayı ve periyodik bakım süreçlerini takip etmeyi amaçlar.

## Roller
- **Bilgi İşlem Sorumlusu / Yönetici:** Birimleri ve cihazları envantere ekler/günceller, bakım periyotlarını takip eder, açılan arızaları uygun teknisyene atar ve genel durumu görüntüler.
- **Teknisyen:** Kendisine atanan veya açık durumdaki arızaları inceler, müdahale ederek arıza durumunu günceller ve yapılan bakım işlemlerini sisteme kaydeder.
- **Birim Kullanıcısı:** Kendi birimindeki cihazlarla ilgili arıza bildiriminde bulunur ve cihaz/arıza durumunu takip eder.

## İş Akışı
1. **Envanter ve Birim Tanımlama:** Sisteme birimler (`Birimler`) ve bu birimlere bağlı cihazlar (`Cihazlar`) seri numarası, tür, alış tarihi ve bakım periyodu bilgileriyle kaydedilir.
2. **Arıza Bildirimi ve Atama:** Bir cihazda sorun oluştuğunda `Arizalar` tablosuna yeni kayıt açılır; sorumlu kişi arızayı ilgili `Teknisyenler` kaydına atar ve durumu günceller.
3. **Bakım ve Durum Takibi:** Periyodik veya arıza sonrası yapılan işlemler `BakimKayitlari` tablosuna işlenir; cihaz bakım süresi ve arıza durumları üzerinden takip edilir.