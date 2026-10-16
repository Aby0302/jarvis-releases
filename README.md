# JARVIS — Kurulum dosyaları

JARVIS kişisel yapay zekâ asistanının Linux ve Windows kurulum dosyaları bu deponun
[Releases](https://github.com/Aby0302/jarvis-releases/releases) bölümünde yayınlanır.

Bu depo ürünün kaynak kodunu içermez. Kaynak geliştirme deposu özeldir.
GitHub'ın otomatik `Source code` arşivleri yalnızca bu dağıtım belgelerini içerir.

İlk masaüstü sürümü x86_64 için önizlemedir. Android paketi henüz yayınlanmamıştır.
Kurulum öncesinde [dağıtım notlarını](DISTRIBUTION.md) okuyun. API anahtarınızı
uygulamanın ilk kurulum ekranında kendiniz girin; paketlerde geliştirici anahtarı yoktur.

Üçüncü taraf bileşenlerin lisans bildirimleri kurulumun `THIRD_PARTY_NOTICES`
dizininde yer alır. Bu bileşenlerin lisansları kendi sahiplerine aittir.

## Kurulum

- Windows: `*-setup.exe` dosyasını çalıştırın.
- Debian/Ubuntu: `.deb` dosyasını paket yöneticinizle kurun.
- Diğer Linux dağıtımları: `*_linux-x64.tar.gz` arşivini çıkarıp içindeki `usr/bin/jarvis` dosyasını çalıştırın. GTK 3 ve WebKitGTK 4.1 gerekir; `usr` dizininin iç yapısını koruyun.

Önizleme Windows paketi henüz yayıncı sertifikasıyla imzalı değildir.
