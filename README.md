<h1 align="center">Aether World Card Wars</h1>

<p align="center">
  Desteni kur, ekipmanını kuşan, yapay zekâya ya da arkadaşına karşı savaş.<br>
  Flutter ile baştan yazılan yeni sürüm · v2.0 · Son güncelleme: Kasım 2026
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

## Son güncelleme (Ekim – Kasım 2026)

v2.0 yayına çıktıktan sonra oyuna eklenenler:

- **100 bölümlük hikâye modu:** Hikâye 20 bölümden 100 bölüme çıktı ve baştan
  sona yazılmış bir senaryoyu izliyor. Bölümlerin 56'sı savaş, kalanı okunan
  anlatı. Her bölümün ne kazandırdığı **Kazanımlar** listesinde görünüyor.
- **Yan hikâyeler:** Ana hikâyeden ayrı ilerleyen, oyuncunun seçimlerine göre
  dallanan ve her biri üç farklı sonla biten görevler.
- **Yeni arayüz:** Mor, kırmızı ve siyah tonlarında, katmanlı yüzeylerden
  oluşan yeni tasarım; yeni ana sayfa düzeni, rütbeye göre değişen kart
  tasarımları ve her seviyeye özel 3D sandık animasyonları.
- **Çoklu dil:** Türkçe, İngilizce ve Çince arayüz.
- **Günlük oyun döngüsü:** Seri ödüllü günlük giriş, şans çarkı, her gün
  değişen **Günün Fırsatı** ve günlük puan sınırı olan antrenman mini oyunları.
- **Efsun ve Mana Taşı:** Eşyalar yeni para birimi Mana Taşı ile
  güçlendiriliyor; başarı şansı sunucuda, eşyanın gücüne ve Demircilik
  seviyesine göre hesaplanıyor.
- **Yetenekler:** Demircilik, silah ustalıkları, okçuluk, büyücülük gibi
  antrenmanla gelişen yetenekler.
- **Ekipman:** Kolye slotu ve set etkileri eklendi.
- **Sosyal:** Arkadaş arama ve ekleme, savaş içi emojiler.
- **Dereceli oyun:** Normal eşleşme, hızlı eşleşme ve meydan okuma.
- **Ses:** Gerçek kayıtlardan savaş sesleri ve retro müzik listesi.
- **Hesap:** Kullanım koşulları, gizlilik ve KVKK metinleri; uygulama içinden
  hesap silme.
- **Yönetim paneli:** Etki kurucusuyla kart düzenleme, denge ölçümü,
  bildirimler, etkinlik yönetimi, raporlar, güncelleme notları ve geri alma.
- **Denge ve performans:** Savunma alt sınırı, ağır kart bonusu gibi savaş
  dengesi ayarları; savaşa girişteki ve savaş alanındaki takılmalar giderildi.

## v1.0 → v2.0: neler değişti?

| | v1.0 (Kotlin) | v2.0 (Flutter) |
|---|---|---|
| Ad | SM CardWars | Aether World Card Wars |
| Platform | Yalnızca Android | Android, iOS, Web (PWA), Windows, macOS, Linux |
| Dil | Türkçe | Türkçe, İngilizce, Çince |
| Deste | 3 kart | 8 kartlık deste, elde sürekli 4 kart (dönüşümlü), 5 deste yuvası |
| Kartlar | 3 çeşit (saldırı, savunma, sersemletme) | Beceri, büyü, pasif kartlar; D'den EX/LG'ye kadar rank sistemi |
| Rakip | Kotlin oyun motorunda olasılıklı yapay zekâ | Hamleleri puanlayan, oyun motoruna gömülü Dart yapay zekâ |
| Çok oyunculu | Yok | Oda koduyla çevrimiçi karşılaşma, dereceli oyun, arkadaşlar |
| İlerleme | Yok | 100 bölümlük hikâye, yan hikâyeler, yetenekler, hesap, ödüller |
| Ekonomi | Yok | Mağaza, Günün Fırsatı, sandıklar, envanter, efsun, Mana Taşı |
| Yönetim | Yok | Ayrı yönetim paneli |

## Öne çıkan özellikler

- **Deste kurma ve kart sistemi:** Beceri, büyü ve pasif kartlar; MP maliyeti,
  şarj süresi, geri tepme ve savunma gibi mekanikler. Bazı kartlar yalnızca
  belirli ekipman, soy veya yetenekle desteye eklenebiliyor.
- **Ekipman ve efsun:** Kask, göğüslük, bacaklık, bot, el ve kolye slotları.
  Eşyalar can, savunma, güç gibi değerler, set etkileri ve yeni kartların
  kilidini açan özellikler veriyor; Mana Taşı ile efsunlanabiliyor. Silahlara
  bağlı "salınım formları" ile savaş sırasında güç kazanılabiliyor.
- **Hikâye modu ve yan hikâyeler:** 100 bölüm boyunca ilerleyen ana hikâye ve
  seçimlere göre dallanan yan görevler; ilerledikçe yeni kart ve eşyalar açılıyor.
- **Yapay zekâ rakip:** Her turda olası hamleleri puanlayıp en iyisini seçen,
  gerektiğinde güçlü bir kart için MP biriktiren bir rakip.
- **Çevrimiçi mod:** Oda oluştur, kodu arkadaşınla paylaş, karşılıklı savaş;
  dereceli eşleşme ve arkadaş listesi.
- **Günlük oyun döngüsü:** Günlük giriş, şans çarkı, antrenman mini oyunları.
- **Mağaza, sandık ve envanter:** Ödüllerle kart ve eşya toplama.
- **Ses ve ayarlar:** Savaş sesleri, müzik, dil seçimi ve kişiselleştirilebilir
  ayarlar.
- **Yönetim paneli:** Kart düzenleyici, denge ayarları ve ölçümü, oyuncu
  yönetimi, ödül kodları, bildirimler ve etkinlikler; içerik uygulamayı
  güncellemeden sunucudan değiştirilebiliyor.

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
| Çoklu dil | Kendi çeviri katmanı (Türkçe, İngilizce, Çince) |
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

v2.0 yayında ve düzenli olarak güncelleniyor.

- Hikâyenin ikinci bölümü ve yeni karakterler hazırlanıyor.
- **Tanrıların Arenası** adlı sınırlı süreli etkinlik modu yolda.
- Mağaza sürümleri (Google Play / App Store) için hazırlık sürüyor.

## Kaynak kod

Kaynak kod özel bir depoda tutuluyor; inceleme için talep üzerine paylaşılabilir.

## İletişim

**osmnnuri** · [Web sitesi](https://osmnnuri.github.io) · [GitHub](https://github.com/osmnnuri) · osmannuriyasar57@gmail.com
