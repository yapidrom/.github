<!--
Issue bağlantısı ZORUNLU. Aşağıdaki satırı düzenle:
  Refs #N     → PR kartı bağlar, KAPATMAZ (K41). Kart Ready for Test → UAT → Production akışını izler;
                sürümü çıkaran kartı Done'a alınca pano issue'yu kapatır.
  Closes #N   → YALNIZ birimsiz ve UAT'siz mekanik PR'da (ref güncellemesi gibi). Başka PR'da
                kullanılırsa kart merge anında Done'a düşer, RfT/UAT/RfP atlanır.
Başka repodaki issue için tam ad: Refs yapidrom/<repo>#N
Muaf: "chore: bump <servis> ref" ve "docs:" başlıklı PR'lar.
PR gövdesinin biçimi tz-core:pr-write skill'indedir.
-->
Refs #
