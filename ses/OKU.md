# SES DOSYALARI

Videoya gömülecek müzik buraya konur. Seçim kuralları → `mark-ses` skill'i.

## Hızlı kural

- **Kaynak:** Meta Sound Collection (facebook.com/sound/collection) ya da
  açıkça ticari lisanslı bir servis. İşletme hesabımız Instagram'ın popüler
  müzik kütüphanesini kullanamaz.
- **Sözsüz.** Ekranda metin var; şarkı sözü okumayla çakışır.
- **Anlattığımız plaktan parça asla.**
- 70-90 BPM civarı, düşük yoğunluklu, drop'suz, zemin gibi duran bir loop.

## Kullanım

Klasörde tek dosya varsa otomatik kullanılır:

```
exports/ses/arsiv_odasi.mp3
```

Birden fazla dosya varsa `CONTENT/video.json` içinde hangisi kullanılacağını
belirt:

```json
{ "ses": "exports/ses/arsiv_odasi.mp3" }
```

Dosya yoksa video sessiz üretilir (script bunu yazar).

## Lisans kaydı

İndirdiğin her parça için kaynağı buraya not et — ileride sorulursa gerekir.

| Dosya | Kaynak | İndirme tarihi | Lisans |
|---|---|---|---|
| | | | |
