# Döviz Çevirici – uzaktan ayarlar

Uygulama her açılışta `config.json` dosyasını okur. Uygulamayı güncellemeden reklamı buradan açıp kapatabilirsiniz.

## Reklamı açmak

1. AdMob’da bir **Banner** reklam birimi oluşturun ve kimliğini kopyalayın (ör. `ca-app-pub-1234567890123456/1234567890`).
2. `config.json` dosyasını GitHub’da düzenleyin:

```json
{
  "ads": {
    "enabled": true,
    "ios": {
      "bannerUnitID": "ca-app-pub-1234567890123456/1234567890"
    }
  }
}
```

3. **Commit changes** ile kaydedin. Değişiklik birkaç dakika içinde uygulamaya ulaşır (uygulama bir sonraki açılışta okur).

Reklamı kapatmak için `"enabled": false` yapın.

> Not: Reklamı ilk kez açmadan önce App Store Connect’teki **App Privacy** (Uygulama Gizliliği) bilgilerini AdMob’un topladığı verilere göre güncelleyin.
