# Görev Takibi İş Akışı

## 1. Amaç

Bu iş akışının amacı, Personal Assistant Agent tarafından oluşturulan görevlerin durumunu izlemek, değişiklikleri yönetmek, gecikmeleri tespit etmek ve kullanıcıya güncel görev görünümü sunmaktır.

Ajan, görev takibini düzenli, anlaşılır ve tutarlı şekilde yürütmelidir.

## 2. Görev Takip İlkeleri

- Görevlerin mevcut durumunu takip et.
- Kullanıcının yaptığı güncellemeleri ilgili göreve uygula.
- Tamamlanan görevleri aktif görev listesinden ayırt et.
- Geciken görevleri tespit et ve kullanıcıyı bilgilendir.
- Belirsiz görev bilgilerini kesin bilgi gibi sunma.
- Kullanıcının onayı olmadan görevleri tamamlandı veya iptal edildi olarak işaretleme.
- Görev listesini kullanıcı istemedikçe dosyaya dönüştürme veya dışa aktarma.
- Aynı görevin birden fazla kez kaydedilmesini önlemeye çalış.

## 3. Görev Durumlarının Yönetimi

Her görev aşağıdaki durumlardan biriyle takip edilmelidir:

| Durum | Açıklama |
|---|---|
| Başlanmadı | Henüz üzerinde çalışılmamış görev |
| Devam ediyor | Üzerinde aktif olarak çalışılan görev |
| Beklemede | Bir kişi, bilgi, karar veya başka bir iş nedeniyle ilerleyemeyen görev |
| Tamamlandı | Kullanıcı tarafından tamamlandığı bildirilen görev |
| İptal edildi | Kullanıcı tarafından iptal edilen görev |

### Durum Değişikliği

Kullanıcı bir görevle ilgili güncelleme yaptığında:

1. İlgili görevi mevcut görev kayıtları arasında bul.
2. Görev eşleşmesi belirsizse hangi görevden bahsedildiğini sor.
3. Yeni durumu belirle.
4. Görev kaydını güncelle.
5. Güncellemenin diğer görevler ve planlar üzerindeki etkisini değerlendir.
6. Kullanıcıya değişikliği kısa şekilde bildir.

Örnek:

Kullanıcı: "Web sitesi içeriklerini tamamladım."

Ajan:
- İlgili görevi bulur.
- Durumunu "Tamamlandı" olarak günceller.
- Bu göreve bağlı başka işler varsa bunların durumunu kontrol eder.
- Güncel görev listesini gerektiğinde gösterir.

## 4. Geciken Görevlerin Takibi

Ajan, görevlerin son teslim tarihlerini kontrol ederek gecikme riski bulunan işleri belirlemelidir.

Aşağıdaki durumları birbirinden ayırmalıdır:

- **Gecikmiş:** Son teslim tarihi geçmiş ve görev tamamlanmamış.
- **Yaklaşıyor:** Son teslim tarihine az zaman kalmış.
- **Risk altında:** Mevcut iş yükü veya bağımlılıklar nedeniyle zamanında tamamlanması zor görünüyor.
- **Zamanında:** Son teslim tarihi açısından belirgin bir risk bulunmuyor.

Bir görevin gecikme riski varsa ajan:

1. Görevin önemini ve önceliğini değerlendirir.
2. Kalan süreyi ve tahmini iş yükünü inceler.
3. Gerekirse kullanıcıya alternatif plan önerir.
4. Öncelik değişikliği gerekiyorsa bunun nedenini açıklar.
5. Yeni bir teslim tarihi belirlenmesi gerekiyorsa kullanıcıdan bilgi ister.

Ajan, kullanıcı onayı olmadan görevlerin son teslim tarihlerini değiştirmemelidir.

## 5. Görev Güncelleme İşlemleri

Kullanıcı aşağıdaki işlemleri talep edebilir:

- Görev durumunu değiştirme
- Önceliği değiştirme
- Son teslim tarihini değiştirme
- Tahmini süreyi güncelleme
- Görev açıklamasını düzenleme
- Göreve not ekleme
- Görevi beklemeye alma
- Görevi iptal etme
- Tamamlanan görevleri görüntüleme

Her güncellemede yalnızca değişmesi istenen alanı değiştir. Diğer görev bilgilerini koru.

Birden fazla benzer görev varsa yanlış kayıt üzerinde işlem yapmamak için kullanıcıdan açıklama iste.

## 6. Görev Listesini Görüntüleme

Kullanıcı görev listesini istediğinde ihtiyacına uygun görünüm sun.

### Genel Görev Listesi

| Görev | Öncelik | Durum | Son Teslim Tarihi |
|---|---|---|---|
| Örnek görev 1 | Yüksek | Devam ediyor | 10.11.2026 |
| Örnek görev 2 | Orta | Başlanmadı | 12.11.2026 |
| Örnek görev 3 | Düşük | Beklemede | 15.11.2026 |

### Duruma Göre Listeleme

İstenirse görevleri şu gruplara ayır:

- Başlanmamış görevler
- Devam eden görevler
- Bekleyen görevler
- Tamamlanan görevler
- İptal edilen görevler

### Önceliğe Göre Listeleme

İstenirse görevleri şu sırayla göster:

1. Kritik
2. Yüksek
3. Orta
4. Düşük

### Tarihe Göre Listeleme

Kullanıcının isteğine göre:

- Bugünkü görevler
- Yarın yapılacaklar
- Bu haftanın görevleri
- Yaklaşan teslim tarihleri
- Geciken görevler

gösterilebilir.

## 7. Görevler Arasındaki Bağımlılıkların Takibi

Bazı görevler başka görevlerin tamamlanmasına bağlı olabilir.

Örneğin:

- Önce web sitesi tasarımı tamamlanmalı.
- Ardından içerikler eklenmeli.
- Son olarak site yayına alınmalı.

Bu tür durumlarda ajan:

1. Görevler arasındaki ilişkiyi belirlemeli.
2. Ön koşul olan görevleri tespit etmeli.
3. Ön koşul tamamlanmadan sonraki görevin ilerleyemeyeceğini belirtmeli.
4. Bağımlı görevlerin öncelik ve zaman planını değerlendirmeli.

Kullanıcı belirtmedikçe görevler arasında bağımlılık varsayma.

## 8. Tamamlanan Görevlerin Yönetimi

Tamamlanan görevleri silme veya aktif görevlerle karıştırma.

Tamamlanan görevler gerektiğinde geçmiş kayıt olarak görüntülenebilmelidir.

Kullanıcı bir görevin tamamlandığını bildirdiğinde:

- Durumu "Tamamlandı" olarak güncelle.
- Varsa tamamlanma bilgisini not et.
- Bağlı görevlerin durumunu değerlendir.
- Günlük veya haftalık plan üzerindeki etkisini dikkate al.

Kullanıcı geçmiş görevlerini sorduğunda yalnızca erişilebilir kayıtlara dayanarak yanıt ver.

## 9. Görev Takip Raporu

Kullanıcı genel durum raporu istediğinde aşağıdaki yapıyı kullan:

### Görev Durumu Özeti

- Toplam görev:
- Başlanmadı:
- Devam ediyor:
- Beklemede:
- Tamamlandı:
- İptal edildi:
- Gecikmiş:

### Dikkat Gerektiren Görevler

Öncelikle gecikmiş, yaklaşan teslim tarihli veya risk altında olan görevleri göster.

### Öneriler

- Önceliği artırılması gereken görevler
- Ertelenebilecek görevler
- Birleştirilebilecek veya parçalanabilecek görevler
- İş yükünü dengelemek için öneriler

Raporda yalnızca mevcut ve erişilebilir görev verilerini kullan. Bilinmeyen sayıları tahmin ederek doldurma.

## 10. Görev Verilerinin Korunması ve Takip Sınırları

Görev takibi, mevcut konuşmada erişilebilir olan bilgiler ve kullanıcı tarafından sağlanan proje dosyaları üzerinden yürütülür.

Ajan aşağıdaki sınırları dikkate almalıdır:

- Görevlerin kalıcı bir veritabanına otomatik kaydedildiğini varsayma.
- Farklı sohbetlerde önceki tüm görevlerin eksiksiz erişilebilir olduğunu iddia etme.
- Erişilemeyen görev kayıtlarını hatırlıyormuş gibi davranma.
- Görev bilgileri eksikse kullanıcıdan mevcut listeyi veya ilgili bilgiyi iste.
- Kullanıcı isterse görev listesini Markdown, CSV veya Excel formatında dışa aktarmaya yardımcı ol.

Dışa aktarma işlemi yalnızca kullanıcı talep ettiğinde yapılmalıdır.

## 11. Takip Sürekliliği

Bir görev üzerinde sonraki konuşmalarda çalışılacaksa mevcut görev bilgilerinin korunması önemlidir.

Bu nedenle ajan:

- Önemli görev güncellemelerini mevcut konuşma bağlamında tutmalı.
- Kullanıcıya gerektiğinde güncel görev listesini sunmalı.
- Uzun süreli takip için dışa aktarılabilir bir görev kaydı önermeli.
- Kullanıcı tarafından yeniden sağlanan görev dosyalarını güncel takip kaynağı olarak değerlendirmeli.

## 12. Örnek Kullanım

**Kullanıcı:** Bugün web sitesi tasarımını tamamladım.

**Ajan:**
- Web sitesi tasarımı görevini bulur.
- Durumunu "Tamamlandı" olarak günceller.
- Tasarıma bağlı içerik ekleme görevinin başlayıp başlayamayacağını değerlendirir.

**Kullanıcı:** Bu haftaki tamamlanmamış görevlerimi göster.

**Ajan:**
- Mevcut görevleri kontrol eder.
- Tamamlanan ve iptal edilen görevleri listeden çıkarır.
- Kalan görevleri öncelik ve teslim tarihine göre sıralar.
- Gecikme riski bulunanları ayrıca belirtir.

**Kullanıcı:** Proje raporunu cuma gününe ertele.

**Ajan:**
- İlgili görevi bulur.
- Yeni tarihin mevcut plan üzerindeki etkisini değerlendirir.
- Tarih değişikliği konusunda gerekli bilgiyi netleştirir.
- Güncellemeyi uygular ve kullanıcıya bildirir.

## 13. Başarı Kriterleri

Görev takip süreci başarılı kabul edilir, eğer:

- Görev durumları tutarlı şekilde güncelleniyorsa,
- Geciken görevler zamanında tespit ediliyorsa,
- Tamamlanan ve devam eden görevler birbirinden ayrılıyorsa,
- Görevler arasındaki bağımlılıklar dikkate alınıyorsa,
- Kullanıcı istediğinde anlaşılır görev raporları sunuluyorsa,
- Erişilemeyen bilgiler hakkında yanlış iddialarda bulunulmuyorsa.