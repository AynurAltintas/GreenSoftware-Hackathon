# Yeşil İşe Alım: Form Tabanlı Sıfır Atık Veri Mimarisi

İki site, aynı sentetik adaylar, gerçek ölçüm.

- **Yeşil sistem (`/`)**: Aday CV yüklemez, formu doldurur. Veri birkaç yüz baytlık JSON olur, eşleştirme Set mantığıyla yapılır.
  CV yalnızca ilk elemeyi geçen adaydan istenir, ayrıştırılmaz.
- **Klasik sistem (`/klasik`)**: Aday PDF CV yükler. Sunucu PDF'i saklar ve senkron ayrıştırır (metin çıkarma, metin yoksa OCR).
  İK her adayı incelemek için PDF'i indirir.
