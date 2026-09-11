# EXAI — sürüm bilgisi

Bu depo yalnızca **sürüm numarasını** tutar. Kaynak kod burada değildir.

`surum.json` üç alan taşır:

| Alan | Ne işe yarar |
|---|---|
| `en_yeni` | Yayınlanmış en son sürüm. Program bundan eskiyse "yeni sürüm var" der ama çalışmaya devam eder. |
| `en_dusuk` | Çalışmasına izin verilen en düşük sürüm. Program bundan eskiyse avlanmayı reddeder. |
| `not` | Kullanıcıya gösterilecek tek cümle (ne değişti). |

## Eski bir sürümü kapatmak

`en_dusuk` alanını yeni sürüme çek ve kaydet. Programlar açılışta buraya
bakar; eski sürümler kendini kapatır.

## Ağ yoksa ne olur

Program çalışmaya **devam eder**. Bu bilinçli: bir internet kesintisi
programı durdurmamalı. Kapı yalnız bu dosya okunup "bu sürüm eski" dediğinde
kapanır.
