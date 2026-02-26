# 🎓 OMÜ Etkinlik Başvuru Formu

Bu proje, **Ondokuz Mayıs Üniversitesi** bünyesinde düzenlenecek teknoloji etkinlikleri için hazırlanmış kapsamlı bir web başvuru formudur. HTML5, CSS3 ve temel JavaScript kullanılarak geliştirilmiştir.

## Proje Özellikleri

Proje, ödev gereksinimlerinde belirtilen tüm modern form elemanlarını ve doğrulama yöntemlerini içermektedir:

* **Kişisel Bilgiler:** Ad-Soyad, Öğrenci No, E-posta, Telefon, Doğum Tarihi ve LinkedIn URL alanları.
* **Etkinlik Tercihleri:** `optgroup` ile gruplandırılmış oturum seçimi, katılım tipi (Radio) ve ilgi alanları (Checkbox).
* **Gelişmiş Alanlar:** CV yükleme (File), Tema rengi seçimi (Color) ve Görüşme saati (Time).
* **İnteraktiflik:** GANO (Range) çubuğu kaydırıldığında değer anlık olarak JavaScript ile güncellenir.
* **Erişilebilirlik:** Tüm alanlar `fieldset` ve `legend` ile gruplandırılmış, her input için `label` (for/id) bağlantısı yapılmıştır.

## Kullanılan Teknolojiler ve Doğrulamalar

- **HTML5:** `required`, `pattern` (Regex), `minlength`, `maxlength` gibi yerleşik doğrulamalar kullanıldı.
- **CSS3:** Responsive (mobil uyumlu) ve kullanıcı dostu bir arayüz tasarlandı.
- **JavaScript:** GANO değerinin anlık gösterimi için DOM manipülasyonu kullanıldı.

## Veri Gönderimi ve Tercih Nedeni

Proje kapsamında **Seçenek 2: Dummy Endpoint'e POST** yöntemi tercih edilmiştir.

> **Neden bu yöntemi seçtim?** > `mailto:` yöntemi kullanıcı cihazına bağımlı olduğu için modern standartlarda verimli değildir. `https://httpbin.org/post` kullanarak verilerin sunucuya nasıl JSON formatında ulaştığını ve `enctype="multipart/form-data"` ile dosya (CV) yükleme işlemlerinin teknik altyapısını gözlemlemek çok daha öğreticidir. Bu yöntem, gerçek API entegrasyonlarını simüle etmek için en sağlıklı yoldur.

## Kullanım
Form doldurulup "Başvuruyu Tamamla" butonuna basıldığında veriler POST edilir ve dönen JSON çıktısı üzerinden veri doğruluğu kontrol edilebilir.

---
**Hazırlayan:** [Pınar Çamoğlu](https://github.com/PinarCamoglu)  
*Ondokuz Mayıs Üniversitesi - Bilgisayar Mühendisliği*