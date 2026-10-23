# Anka Fantasy Football - Draft Asistanı 2025

12 takımlı, PPR, snake formatındaki bir fantasy football ligi için hazırlanmış, tek bir HTML dosyasından oluşan draft asistanı. 2025 sezonu oyuncu sıralamalarını, bye haftalarını ve uzman notlarını dosyanın içinde taşır; draft sırasında seçimleri tahtaya işler ve kendi takımın için öneri üretir. Sunucu, kurulum ya da derleme gerektirmez.

## Özellikler

- **Snake draft tahtası:** 12 takım × 18 tur. Her seçim ("Draft Et" düğmesi) tahtaya işlenir, sırası gelen takım vurgulanır. Tam ve sıkıştırılmış görünüm arasında geçiş yapılabilir.
- **"Benim Sıram" seçimi:** Draft sırasındaki herhangi bir takımı kendi takımın olarak seçersin; öneriler ve kadro özeti o takıma göre hesaplanır.
- **Öneri paneli** (her pickte en fazla 4 blok):
  - **BPA:** Mevcut en iyi oyuncular, varsa uzman notuyla.
  - **Pozisyon ihtiyacı:** Kadrondaki eksik pozisyona göre öneri.
  - **Düşen değerler (ADP fırsatı):** Sıralamasına göre beklenenden geç kalan oyuncular.
  - **Radardaki uykucular:** 6. turdan sonra, uzman notunda "sleeper" olarak geçen oyuncular.
- **Oyuncu listesi:** 324 oyuncu (QB, RB, WR, TE, K, DEF); genel sıra, pozisyon sırası (ör. RB5), takım, bye haftası ve durum etiketi (Q, IR, SUS, PUP, D). İsim/takım araması ve pozisyon filtresi; liste ADP'ye göre sıralanır ve ilk 100 müsait oyuncu gösterilir.
- **Kadro özeti:** Seçtiğin takımın pozisyon dağılımı (QB/RB/WR/TE/K/DEF).

## Teknoloji yığını

- Tek dosya: HTML + vanilla JavaScript
- Tailwind CSS (CDN: `cdn.tailwindcss.com`)
- Google Fonts (Inter, Playfair Display)

Stil ve yazı tipleri CDN'den yüklendiği için sayfa açılırken internet bağlantısı gerekir.

## Klasör yapısı

```
nfl-fantasy-draft-assistant-2025/
├── nfl-fantasy-2025.html   # Uygulamanın tamamı (arayüz, veri, öneri mantığı)
└── README.md
```

Dosya içindeki ana parçalar:

- `DRAFT_ORDER`: Ligdeki 12 takımın draft sırası (sabit takım adları).
- `ALL_PLAYERS_DATA`: Oyuncu verisi (`rank`, `name`, `position`, `team`, `status`, `bye`, `adp`).
- `EXPERT_TAKES`: Oyuncu adına göre uzman notları.
- `getAdvancedRecommendations()`: Öneri mantığı.

## Kullanım

1. `nfl-fantasy-2025.html` dosyasını modern bir tarayıcıda aç.
2. "Benim Sıram" menüsünden kendi takımını seç.
3. Draft ilerledikçe seçilen oyuncuları listeden "Draft Et" ile işaretle; tahta, kadro özeti ve öneriler her pickte güncellenir.

Başka bir lig için kullanmak istersen `DRAFT_ORDER` dizisindeki takım adlarını düzenlemen yeterlidir. Draft durumu tarayıcıda saklanmaz; sayfa yenilenirse draft sıfırlanır.

## Veri kaynakları

Oyuncu sıralamaları, ADP'ler ve uzman notları çeşitli uzman kaynaklarından (CBS Sports, FantasyPros, Flock Fantasy, The Fantasy Footballers, BDGE, NFL.com vb.) elle derlenip dosyaya gömülmüştür. Bye haftaları 2025 NFL takvimine göredir. Uygulama çalışırken dış bir veri kaynağına bağlanmaz.

## Proje durumu

2025-08-31 tarihinde, 2025 sezonu draftı için tek günde hazırlandı (3 commit). Bu sürüm artık geliştirilmiyor; 2026 sezonu için yeniden yazılan sürüm ayrı bir repodadır: [`nfl-draft-asistant-2026`](https://github.com/muhammetaliyoldar/nfl-draft-asistant-2026). Repoda `LICENSE` dosyası yoktur.

---

<p align="center"><em>Ze'O tarafından geliştirildi.</em></p>
