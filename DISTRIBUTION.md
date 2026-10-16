# JARVIS 0.1.0 — masaüstü önizleme

Uygulama kaynak kodu içermez; ürünün Python modülleri yerel uzantılara derlenmiştir.
Kaynak depo özeldir. Tersine mühendisliğe karşı mutlak koruma vaat edilmez.

Kurulum Python veya kaynak klasörü gerektirmez. İlk açılışta kendi sağlayıcını ve
gerekiyorsa kendi API anahtarını gir. Geliştiricinin anahtarı, sohbeti veya hafızası
pakete dahil edilmez. Yerel modeller için ayrıca Ollama kurulmalıdır.

İsteğe bağlı araçlar:

- Konuşmayı yazıya çevirme: ffmpeg PATH içinde olmalı; Whisper modeli ilk kullanımda indirilir.
- Yerel ses: ayrı kurulan Piper CLI ve ses modelleri ya da espeak-ng gerekir.
  Piper model dizini `JARVIS_VOICES` veya kullanıcı veri dizinindeki `voices/` klasörüdür.
- İnternet üzerinden ses: ayarlardan Edge seçilirse okunacak metin Microsoft'a gönderilir.
- Tarayıcı araçları: Chromium veya Chrome kurulu olmalı.
- Android cihaz kontrolü: adb kurulu ve USB hata ayıklama izni verilmiş olmalı.
- Belge görselleri: LibreOffice kurulu olmalı. PDF Türkçe yazı tipi için DejaVu Sans kur.
- Kodda arama: `rg` (ripgrep), alternatif olarak `grep`, PATH içinde bulunmalı.

Bu önizleme Piper'ın GPL kitaplığını veya lisansı ayrıca değerlendirilmesi gereken
uyandırma kelimesi modellerini içermez. "Hey Jarvis" bu pakette etkin değildir.
Linux'ta paket yöneticinle; Windows'ta araçların resmi dağıtımlarıyla ek araçları kur.
Windows kurulum dosyası henüz bir yayıncı sertifikasıyla imzalı değildir.

Veri dizinleri: Linux `$XDG_DATA_HOME/Jarvis` (varsayılan `~/.local/share/Jarvis`),
Windows `%LOCALAPPDATA%/Jarvis`. Her iki platformda `JARVIS_DATA_DIR` ile değiştirilebilir.
Üçüncü taraf bildirimleri `THIRD_PARTY_NOTICES` dizinindedir.

Linux'ta `.deb` paketini destekleyen dağıtımlarda paket yöneticinle kur.
Taşınabilir `.tar.gz` sürümünü çıkardıktan sonra `usr/bin/jarvis` dosyasını çalıştır;
GTK 3 ve WebKitGTK 4.1 sistemde bulunmalıdır. `usr/bin` ve `usr/lib` dizinlerini birlikte taşı.
