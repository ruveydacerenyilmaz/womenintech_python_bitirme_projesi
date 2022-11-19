# Women in Tech Akademi-Python Eğitimi Bitirme Projesi
<h3 align="center"> <h1 align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com/?lines=Keyifli+İncelemeler!&center=true&size=25">
  </a> 

![gif](https://media.giphy.com/media/26ufmepVftH5Y2V7q/giphy.gif)
</h3>

# SistersLab Bilim ve Teknolojide Kadın Derneği tarafından düzenlenen Women In Tech Akademisi sonunda, Python Bitirme Projesi olarak "1896 ile 2016 Yılları Arasında Oynanan Olimpiyat Oyunları" ile ilgili veri analizi yapıldı. 

* Her iki etkinlik son olarak 1992'de aynı yıl içerisinde gerçekleştirildi ve 1994'te düzenlenen Kış Olimpiyatları ile birlikte iki etkinlik arasında ikişer yıllık fark oluştu.

# Analiz esnasında kullanılan dosyalar;
- athlete_events.csv
- noc_region.csv

# Analiz yapılırken Kullanılan kütüphaneler;
- Pandas, 
- Numpy, 
- Matplotlib, 
- Seaborn, 
- Missingno kütüphnelerinden yararlanılmıştır.

# Veri setindeki sütunların bilgisi;
* ID - Her sporcu için benzersiz numara, kimlik gibi düşünülebilir.
* Name - Sporcunun adı ve soyadı bilgis bir aradadır.
* Sex - M ya da F --> M: Male(Erkek) & F: Female(Kadın)
* Age - Yaş Bilgisi (Tamsayı olarak)
* Height - Santimetre Cinsinden
* Weight - Kilogram Cinsinden
* Team - Takım Adı
* NOC - Ulusal Olimpiyat Komitesi 3 harfli kod (Örn: Turkey-> TUR)
* Games - Yıl ve Olimpiyat Oyununun Sezonu 
* Year - Oynanılan Yıl (Tamsayı olarak)(Örn: 1912, 2014)
* Season - Summer ya da Winter (Oynanılan Olimpiyat Sezonu (Yaz veya Kış Olimpiyatı))
* City - Olimpiyatlara Ev Sahipliği Yapan Şehir
* Sport - Spor Dalı
* Event - Etkinlik (Basketbol dalında Erkeklerin Oynadığı Basketbol Oyunu)
* Medal - Gold, Silver, Bronze, ya da NaN (Altın, Gümüş, Bronz Madalyalar ve NaN değerlerden oluşmakta.)
--------------------------

# Veri Seti İçerisinde Yapılan İşlemler;
* Veri setleri tanımlandıktan sonra sütunlar ve değerleri incelendi,
* İki veri seti  ortak sütunlarıyla birleştirildi,
* Sayısal değerler içeren sütunlardan bazı farkı bilgiler elde edildi,
* Tekrar eden satırlar veri setinden kaldırıldı,
* Veri seti içerisinde eksik verilerin sayıları belirlendi, bu değerlerden bazıları dolduruldu ya da silindi, 
* Hem grafikler için hem de analiz için group by işlemleri yapıldı,
* Grafik olarak pairplot, korelasyon grafiği , line, bar, pie, boxplot grafik yöntemleri kullanıldı.

# Yapılan Analizler:
1. Ülkelerin Kazandığı Altın Madalya Sayısı

    * En çok 'Gold' madalya kazanan ülke: USA - 2115 Gold Madalya 

2. Yarışmacıların Kazandığı Madalya Sayısı

    * En çok madalya kazanan yarışmacı: Michael Fred Phelps - 28 madalya kazanmıştır.

3. Belirli Bir Dalda Yarışan Sporcuların Boy-Kilo Ortalaması
    * 'Figure Skating' kategorisi incelendi.

4. Spor Dallarına Göre Kadın-Erkek Oranı

    * En çok katılımın olduğu spor dalı: Athletics, 2414 Erkek, 1239 Kadın katılımcısı olmuştur.
    * En az katılımın olduğu spor dalı: Art Competitions, 2 Erkek ve 0 Kadın katılımcısı olmuştur.

5. Belli Bir Spor Dalında Katılımcıların Kazandığı Madalya Sayısı
    * 'Figure Skating' Kategorisinde;
        - En çok madalya kazanan katılımcı; Yevgeny Viktorovich Plyushchenko 4 madalya kazanmıştır.

6. Yaz ve Kış Olimpiyatlarındaki Katılımcıları İnceleme 
    * Olimpiyat Verisindeki Tüm Madalya Sayıları
    * Yaz Olimpiyatlarında;
        - Kazanılan Toplam Madalya Sayıları
        - Yaz Olimpiyatlarında Kazanılan Madalyaların Cinsiyete Göre Dağılımı
        - Yaz Olimpiyatlarına Katılan Kişilelerin Boy ve Kilosunun Cinsiyete Göre Grafiği
    * Kış Olimpiyatlarında;
        - Kazanılan Toplam Madalya Sayıları
        - Kış Olimpiyatlarında Kazanılan Madalyaların Cinsiyete Göre Dağılımı
        - Kış Olimpiyatlarına Katılan Kişilenlerin Boy ve Kilosunun Cinsiyete Göre Grafiği

7. Yıllara Göre Katılımcıların Cinsiyet Durumu

    * 1896-2016 yılları arasında katılan katılımcıların; 
        - %65.7'si Erkek 
        - %34.3'ü Kadın
8. Birkaç Farklı Filtreleme İşlemleri

    * 18 yaşından küçük altın madalyaya sahip 344 katılımcı varmış.
    * Aynı kişiler olsa bile, düzenlenmiş veri seti içinde Türkiye'den 72 katılımcı varmış.
    * Türkiye'den olimpiyatlara 'Weightlifting' (Ağırlık Kaldırma-Halter Kaldırma) kategorisinde 30 katılımcı olmuştur.
    * Önemli olayların olduğu yıllardaki olimpiyatları listelemek istedim ama o dönemlerde yapılmamış.
        * 1916'da Berlin'de yapılması planlanan olimpiyat oyunları, Birinci Dünya Savaşı nedeniyle iptal edildi.
        * IOC, 5-8 Nisan 1919'da yaptığı toplantıda savaşın sorumlusu olarak gördüğü Almanya, Avusturya, Macaristan, Bulgaristan ve Osmanlı Devleti'nin 1920 Anvers Olimpiyat Oyunları'na çağrılmamasına karar verdi.
        * 1940 Tokyo ve 1944 Londra Olimpiyat Oyunları, 2. Dünya Savaşı nedeniyle yapılamadı.
    * SSCB dağılmadan katılımcıların katıldığı farklı olimpiyat oyunları en yakın tarihten geçmişe doğru sıralanmıştır.
    
