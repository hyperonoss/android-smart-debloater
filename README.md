# Android Smart Debloater

Android cihazlardaki gereksiz ve dikkat gerektiren paketleri açıklamalarıyla incelemenizi sağlayan portable Windows uygulaması.

Amaç, teknik bilgisi olmayan kullanıcıların bir paketi kaldırmadan önce:

- Ne işe yaradığını
- Kaldırılırsa hangi özelliğin kaybolabileceğini
- Paketin ne kadar güvenilir olduğunu
- Kullanıcı tarafından yüklenmiş bir uygulama olup olmadığını

anlayabilmesidir.

## İndirme

GitHub Releases bölümünden şu dosyalardan birini indirin:

- `AndroidDebloater.exe`: Tek dosyalık portable sürüm
- `AndroidDebloater.zip`: EXE ve veri klasörü içeren portable paket

Kurulum gerekmez.

## Kullanım

1. Telefonunuzda Geliştirici Seçenekleri’ni açın.
2. USB hata ayıklamayı etkinleştirin.
3. Telefonu USB kablosuyla bilgisayara bağlayın.
4. Telefonda çıkan bilgisayar bağlantısı iznini onaylayın.
5. `AndroidDebloater.exe` dosyasını çalıştırın.
6. Paket açıklamalarını okuyup yalnızca kaldırmak istediğiniz paketleri seçin.

## Güvenlik yaklaşımı

- Kritik Android sistem paketleri kilitlidir.
- Varsayılan Telefon, Mesajlar ve Ana ekran uygulamaları korunur.
- Bilinmeyen paketler başlangıç listesine eklenmez.
- Kullanıcı tarafından yüklenen uygulamalar bloatware olarak işaretlenmez.
- Reklam ve telemetri paketleri ayrı açıklanır.
- Gelişmiş ve yeterince doğrulanmamış paketler seçilemez.
- Paket açıklamalarında olası özellik kayıpları açıkça belirtilir.

Her cihazın üreticisi, modeli ve Android sürümü farklı olduğu için kaldırma işlemi öncesinde açıklamaları mutlaka okuyun. Önemli verilerinizi önceden yedekleyin.

## Desteklenen cihazlar

İlk doğrulama çalışmaları şu Android 16 cihazlarıyla yapılmaktadır:

- Honor 200
- Samsung Galaxy S24 FE
- Tecno Camon 40 Pro 5G
- Xiaomi 15T

Diğer Android cihazlarında paketlerin etkisi farklı olabilir.

## Güncelleme denetimi

Uygulama açılışta GitHub Releases bölümünü kontrol eder. Yeni sürüm bulunduğunda uygulama içinden doğrudan indirme bağlantısı gösterir.

Güncelleme deposu ayarı:

```text
data/update_config.json
```

```json
{
  "repository": "hyperonoss/android-smart-debloater"
}
```

## Debloat profilleri

Uygulama, kaldırma tercihlerini cihaz modeli ve Android sürümüyle birlikte profil olarak kaydedebilir. Bu profiller:

- Telefonun Wi-Fi ayarlarını
- Bildirim ayarlarını
- İzinleri
- Diğer sistem ayarlarını

yedeklemez.

Android güncellemesinden sonra kaydedilmiş paket listesini yeniden inceleyin. Eski profil yeni Android sürümünde otomatik olarak uygulanmaz.

## Geri bildirim

Kullanıcılar paketler hakkında yan etki veya kullanım deneyimi bildirebilir. Geri bildirimler varsayılan olarak bilgisayarda yerel olarak saklanır.

Geliştiriciye cihaz ve paket bilgisi gönderilmesi için kullanıcıdan ayrıca açık onay alınır.

## Lisans ve kaynaklar

Paket açıklamaları; üretici verileri, Android bilgileri, Universal Android Debloater listeleri ve elle düzenlenmiş Türkçe açıklamalardan oluşturulmuştur.

Bu uygulama Android’in resmi bir aracı değildir.
