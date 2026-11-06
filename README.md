# Yörünge

3D odak ve alışkanlık evreni. Her alışkanlık, merkezdeki odak yıldızının çevresinde dönen bir gezegendir. Bir gezegen için odak seansı (Pomodoro) başlattığında yıldızdan gezegene spiral bir parçacık akışı başlar. Seans bitince gezegen büyür, parlar ve yörüngesine yeni bir ay girer. 3, 7 ve 30 günlük serilerde gezegenin çevresinde halkalar belirir.

**Canlı:** https://zeynepkaya28.github.io/yorunge/

## Özellikler

- Three.js 0.160 sahne: 4500 noktalı yıldız alanı (parallax), shader'lı nabız atan yıldız, bloom, ACES tonemapping, sis
- Fresnel atmosferli gezegenler; boyut toplam odak dakikasına göre yumuşakça büyür
- Hover etiketi, tıklayınca kamera gezegene uçar ve onu takip eder
- Alışkanlık ekle, yeniden adlandır, sil; 8 renklik palet
- 25 / 50 dk ya da özel süreli zamanlayıcı, dairesel ilerleme halkası, 60× hızlı demo modu
- Tamamlanınca şok dalgası, yeni ay, seri hesabı ve seri halkaları
- localStorage kaydı (`yorunge.v1`), veri yoksa örnek evrenle açılır
- Son 14 günün yığılmış sütun grafiği, toplam saat, rekor seri
- Klavye: `Space` başlat/duraklat, `1–9` gezegen seç, `Esc` genel görünüm
- Mobilde paneller alttan açılan çekmeceye dönüşür; `prefers-reduced-motion` desteği

## Çalıştırma

Derleme adımı yok. `index.html` dosyasını tarayıcıda açman yeterli (Three.js jsDelivr'den yüklenir, internet gerekir).

## Veri şeması

```json
{ "habits": [ { "id": "", "name": "", "color": "#6f9bff", "minutes": 0, "sessions": [ { "t": 0, "min": 25 } ], "moons": 0 } ] }
```
