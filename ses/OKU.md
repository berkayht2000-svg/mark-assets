# SES DOSYALARI

Videoya gömülecek ses buraya konur. Kurallar → `mark-ses` skill'i.

## Varsayılan: sesi kendimiz üretiyoruz

```bash
python TECHNICAL/ses_uret.py
```

Çıktı: `exports/ses/mark_zemin_<video>.wav` — tempo videoya kilitli, boom
bap davulu, odun çıtırtısı ve oda tonuyla. `video_uret.py` **o videoya ait**
dosyayı adından bulup gömer. Telif tartışması yok; ses tamamen bizim.

**Her videonun sesi ayrı dosyada.** Önceden hepsi tek `mark_zemin.wav`'a
yazılıyordu ve her yeni video öncekinin sesini siliyordu; eski bir video
yeniden render edilirse yanlış sesi kapıyordu.

Başka bir varyasyon istersen tohumu değiştir:

```bash
python TECHNICAL/ses_uret.py --sure 30 --tohum 9
```

Beğendiğin tohumu not et — aynı tohum aynı sesi verir.

## Dışarıdan ses alınacaksa

- **Kaynak:** Meta Sound Collection (facebook.com/sound/collection) ya da
  açıkça ticari lisanslı bir servis. İşletme hesabımız Instagram'ın popüler
  müzik kütüphanesini kullanamaz.
- **Sözsüz.** Ekranda metin var; şarkı sözü okumayla çakışır.
- **Anlattığımız plaktan parça asla.**

Klasörde birden fazla dosya varsa `CONTENT/video.json` içinde belirt:

```json
{ "ses": "exports/ses/mark_zemin.wav" }
```

## Lisans kaydı (yalnız dışarıdan alınanlar için)

| Dosya | Kaynak | İndirme tarihi | Lisans |
|---|---|---|---|
| | | | |

> Ham ses dosyaları public `mark-assets` reposuna girmiyor (`.gitignore`) —
> lisanslar sesi içerikte kullanmaya izin verir, dosyayı yeniden dağıtmaya
> değil. Kendi ürettiğimiz ses için bu kısıt yok ama gereksiz, ses videoya
> gömülü zaten gidiyor.
