<h1 align="center">Aether World Card Wars</h1>

<p align="center">
  Desteni kur, ekipmanını kuşan, yapay zekâya ya da arkadaşına karşı savaş.<br>
  Flutter ile baştan yazılan yeni sürüm · v2.0 ve sonrası
</p>

<p align="center">
  <a href="https://osmnnuri.github.io"><b>Güncel görseller için siteme göz at</b></a>
</p>

---

> Oyunun eski adı **SM CardWars (Strategy Master Card Wars)** idi. v2.0 ile
> birlikte adı **Aether World Card Wars** olarak değiştirildi.

## Oyun konsepti

Aether World Card Wars, sıra tabanlı ve taktik ağırlıklı bir kart savaşı oyunu.
Oyuncu kartlarından **8 kartlık bir deste** kurar, ekipmanlarıyla karakterini
güçlendirir ve rakibini yenmeye çalışır.

Savaş sırasında oyuncunun elinde her zaman **4 kart** bulunur. Oynanan kartın
yerine desteden yeni bir kart gelir; 8 kart sürekli dönüşümlü olarak kullanılır.
Böylece her turda hem eldeki kartları hem de sıradaki kartları düşünerek MP'yi
hangi karta harcayacağına karar vermek gerekir.

İlk sürüm (v1.0) Kotlin ile yazılmış, üç kartlık basit bir demoydu. v2.0'da
oyun Flutter ile sıfırdan yeniden yazıldı ve kapsamı büyük ölçüde genişledi.

## v1.0 → v2.0: neler değişti?

| | v1.0 (Kotlin) | v2.0 (Flutter) |
|---|---|---|
| Ad | SM CardWars | Aether World Card Wars |
| Platform | Yalnızca Android | Android, iOS, Web (PWA), Windows, macOS, Linux |
| Deste | 3 kart | 8 kartlık deste, elde sürekli 4 kart (dönüşümlü) |
| Kartlar | 3 çeşit (saldırı, savunma, sersemletme) | Beceri, büyü, pasif kartlar; D'den EX/LG'ye kadar rank sistemi |
| Rakip | Kotlin oyun motorunda olasılıklı yapay zekâ | Hamleleri puanlayan, oyun motoruna gömülü Dart yapay zekâ |
| Çok oyunculu | Yok | Dereceli oyun, oda koduyla çevrimiçi karşılaşma, arkadaş sistemi |
| İlerleme | Yok | 100 bölümlük hikâye modu, dallanan yan hikâyeler, yetenekler, hesap |
| Ekonomi | Yok | Mağaza, Günün Fırsatı, sandıklar, Mana Taşı, efsun, envanter |
| Dil | Türkçe | Türkçe, İngilizce, Çince |
| Yönetim | Yok | Ayrı yönetim paneli |

## Öne çıkan özellikler

- **Deste kurma ve kart sistemi:** Beceri, büyü ve pasif kartlar; MP maliyeti,
  şarj süresi, geri tepme ve savunma gibi mekanikler. Bazı kartlar yalnızca
  belirli ekipman, soy veya yetenekle desteye eklenebiliyor.
- **Ekipman ve efsun:** Kask, göğüslük, bacaklık, bot, el ve kolye slotları.
  Eşyalar can, savunma, güç gibi değerler, set etkileri ve yeni kartların
  kilidini açan özellikler veriyor. Eşyalar Mana Taşı ile efsunlanabiliyor;
  başarı şansı sunucuda, güce ve Demircilik seviyesine göre hesaplanıyor.
- **Hikâye modu:** Baştan sona bir senaryoyu izleyen 100 bölüm; 56'sı savaş,
  kalanı okunan anlatı. Her bölümün ne kazandırdığı "Kazanımlar" listesinde
  görünüyor.
- **Yan hikâyeler:** Ana hikâyeden ayrı ilerleyen, seçimlere göre dallanan ve
  her biri üç farklı sonla biten görevler.
- **Yapay zekâ rakip:** Her turda olası hamleleri puanlayıp en iyisini seçen,
  gerektiğinde güçlü bir kart için MP biriktiren bir rakip.
- **Çevrimiçi ve sosyal:** Dereceli oyun (normal eşleşme, hızlı eşleşme,
  meydan okuma), oda koduyla karşılıklı savaş, arkadaş arama ve savaş içi
  emojiler.
- **Günlük oyun döngüsü:** Seri ödüllü günlük giriş, şans çarkı, her gün
  değişen Günün Fırsatı ve günlük puan sınırı olan antrenman mini oyunları.
  Mini oyunlar yetenek seviyelerini (Demircilik, silah ustalıkları vb.)
  yükseltiyor.
- **Mağaza, sandık ve envanter:** Seviyeye göre fiyatlanan ekipman, her
  seviyeye özel 3D sandık animasyonları, rütbeye göre değişen kart tasarımları.
- **Arayüz ve ses:** Mor, kırmızı ve siyah tonlarında katmanlı arayüz; gerçek
  kayıtlı (CC0) savaş sesleri ve retro müzik listesi.
- **Çoklu dil:** Türkçe, İngilizce ve Çince arayüz.
- **Hesap:** Kullanım koşulları, gizlilik ve KVKK metinleri; uygulama içinden
  hesap silme.
- **Yönetim paneli:** Etki kurucusuyla kart düzenleme, denge ölçümü, oyuncu
  yönetimi, bildirimler, etkinlikler, raporlar, güncelleme notları ve geri
  alma; içerik uygulamayı güncellemeden sunucudan değiştirilebiliyor.

## Neden Kotlin'den Flutter'a geçtim?

- **Çapraz platform:** Tek kod tabanıyla Android, iOS, web ve masaüstü için
  derleme yapabiliyorum. v1.0 yalnızca Android'de çalışıyordu.
- **Sektördeki yeri:** Flutter mobil geliştirme alanında güçlü bir konumda ve
  daha fazla iş imkânı sunuyor; bu projeyi o yönde kendimi geliştirmek için
  de kullanıyorum.
- **Aktif kullanım:** Şu anda başka projelerimi de Flutter ile yürüttüğüm için
  bu ekosisteme ve Dart'a daha yatkınım.
- **PWA esnekliği:** Flutter'ın web desteği sayesinde oyunu PWA olarak
  yayınlayabiliyorum. Herhangi bir mağazaya bağlı kalmadan tarayıcıdan
  açılabiliyor ve ana ekrana eklenerek mobil uygulama gibi kullanılabiliyor.

## Kullanılan teknolojiler

| Katman | Teknoloji |
|---|---|
| Uygulama | Flutter, Dart |
| Çoklu dil | Kendi `t()` çeviri katmanı (tr / en / zh) |
| Yerel veri | shared_preferences |
| Ses | audioplayers |
| Ağ | http |
| Sunucu | Node.js (serverless API), Zod ile doğrulama |
| Veritabanı | Firebase (firebase-admin) |
| Barındırma | Firebase Hosting (web / PWA), Vercel (API), Netlify (API vekil sunucusu) |
| Test | flutter_test, node:test |

## Tasarım ve görseller

Oyun görselleri yapay zekâ ile üretildi; bunun dışındaki tasarım ve düzen bana
ait. Kodlama sürecinde yapay zekâ destekli araçlardan yararlandım.

## Durum ve yol haritası

Oyun yayında ve düzenli güncelleniyor; her güncellemenin notları oyun
içinde gösteriliyor.

- Hikâyenin ikinci bölümü (yeni senaryo, yeni karakter ve kartlar) hazırlanıyor.
- Tanrıların Arenası adlı sınırlı süreli etkinlik modu geliyor.
- Hikâye metninin İngilizce ve Çince çevirisi yapılacak.
- Mağaza sürümleri (Google Play / App Store) için hazırlık sürüyor.

## Kaynak kod

Kaynak kod özel bir depoda tutuluyor; inceleme için talep üzerine paylaşılabilir.

## İletişim

**osmnnuri** · [Web sitesi](https://osmnnuri.github.io) · [GitHub](https://github.com/osmnnuri) · osmannuriyasar57@gmail.com
