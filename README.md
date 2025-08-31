# Anka Fantasy Football - Draft Asistanı 2025

![Status](https://img.shields.io/badge/Status-Tamamland%C4%B1-brightgreen)
![Versiyon](https://img.shields.io/badge/Versiyon-1.0.0-blue)
![Teknoloji](https://img.shields.io/badge/Teknoloji-HTML/CSS/JS-orange)
![Framework](https://img.shields.io/badge/Framework-TailwindCSS-38B2AC)

*Mükemmel draft'ınız için ihtiyacınız olan tek yardımcı. Veri ve uzman analizlerini birleştiren akıllı asistan.*


## 📝 Proje Hakkında

**Anka Fantasy Football Draft Asistanı**, 12 takımlı, PPR (Puan Başına Yakalama) ve Snake Draft formatındaki fantezi futbol ligleri için özel olarak tasarlanmış, web tabanlı bir yardımcı araçtır. Bu proje, standart oyuncu sıralamalarının ötesine geçerek, onlarca farklı uzmanın analizlerini, oyuncu kademelerini (tiers), uyuyan (sleeper) potansiyellerini ve risk faktörlerini tek bir akıllı algoritma altında birleştirir.

Draft sırasında size sadece "kimin en iyi olduğunu" değil, aynı zamanda takımınızın ihtiyacına, draft'ın gidişatına ve uzmanların ortak görüşüne göre **en stratejik hamlenin ne olduğunu** gösterir.

## ✨ Ana Özellikler

* **📊 Dinamik Draft Tahtası:**
    * 12 takımlı `snake` draft formatını tam olarak simüle eder.
    * Yapılan her seçimi anlık olarak tahtaya işler ve tüm arayüzü günceller.
    * O an sırası gelen takımı görsel olarak öne çıkarır.

* **🧠 "Mükemmel Seçim Algoritması" - Akıllı Öneriler:**
    * **BPA (En İyi Mevcut Oyuncu):** O anki en yüksek potansiyele sahip oyuncuları, ilgili **uzman notlarıyla** birlikte sunar.
    * **Pozisyon İhtiyacı:** Kadronuzdaki eksiklikleri sürekli analiz eder ve en kritik pozisyondaki en iyi oyuncuları önerir.
    * **ADP Fırsatları:** Sıralamasına göre beklenenden daha alt sıralara düşmüş, "kelepir" olarak nitelendirilebilecek oyuncuları size bildirir.
    * **Uzmanların Gözdesi & Uykucular (Sleepers):** Draft'ın turuna göre, uzmanların "mutlaka alın" veya "gizli potansiyel" olarak işaretlediği oyuncuları öne çıkarır.
    * **Strateji Tespiti:** Yaptığınız seçimlere göre uyguladığınız stratejiyi (örn: "Hero RB", "Zero RB") analiz eder ve bu stratejinin bir sonraki adımı için en mantıklı oyuncuları önerir.

* **📈 Gelişmiş Oyuncu Listesi:**
    * **Hibrit Sıralama:** 300'den fazla oyuncuyu, uzman analizleri ve puan beklentilerine dayalı "optimum" bir genel sıralama (`Genel Rank`) ile sunar.
    * **Pozisyonel Sıralama:** Her oyuncunun kendi pozisyonu içindeki sırasını (`Pozisyon Rank: RB5, WR12 vb.`) göstererek karar vermeyi kolaylaştırır.
    * **Filtreleme ve Arama:** Oyuncuları isme veya pozisyona göre (QB, RB, WR, TE, K, DEF) anında filtreleyebilirsiniz.
    * **Kritik Bilgiler:** Her oyuncu kartında güncel **Bye Haftası** ve sakatlık/ceza **Durumu** (Q, SUS, IR) bilgisi yer alır.

* **👤 Kişiselleştirilmiş Takım Paneli:**
    * Draft'taki herhangi bir takımı "Benim Sıram" olarak seçebilir ve tüm önerileri o takımın perspektifinden alabilirsiniz.
    * Seçtiğiniz takımın anlık **Kadro Dağılımını** (1 QB, 2 RB vb.) dinamik olarak takip edebilirsiniz.

## 🛠️ Teknoloji Mimarisi

Bu proje, modern web teknolojileri kullanılarak, herhangi bir sunucu ihtiyacı olmadan tamamen tarayıcı üzerinde çalışacak şekilde tasarlanmıştır.

* **HTML5:** Uygulamanın temel yapısı.
* **Tailwind CSS:** Hızlı, modern ve şık bir arayüz için kullanılan CSS framework'ü.
* **JavaScript (ES6):** Uygulamanın tüm dinamik işlevselliğini, draft simülasyonunu ve akıllı öneri algoritmasını yöneten ana programlama dili.

## 🚀 Kurulum ve Kullanım

Bu aracın kurulumu yoktur. Anında kullanmaya başlayabilirsiniz.

1.  Proje dosyasını (`.html` uzantılı) bilgisayarınıza indirin.
2.  Dosyayı Google Chrome, Firefox veya herhangi bir modern web tarayıcısı ile açın.
3.  Draft'ınız başladığında, "Benim Sıram" menüsünden kendi takımınızı seçin ve draft ilerledikçe seçimleri arayüz üzerinden yapın. Asistan size her adımda rehberlik edecektir.

## 📚 Veri Kaynakları ve Teşekkür

Bu projenin beynini oluşturan oyuncu veritabanı ve stratejik analizler, **Ze'O** tarafından titizlikle derlenen onlarca farklı kaynaktan (CBS Sports, FantasyPros, Flock Fantasy, The Fantasy Footballers, BDGE, NFL.com vb.) alınmıştır. Tüm veriler, bu kaynaklardaki uzman görüşleri, 2025 sezonu fantezi puanı projeksiyonları ve güncel sıralamalar harmanlanarak oluşturulmuştur.

Bye Haftası verileri güncel **2025 NFL takvimine** göredir.

---

<p align="center">
  <em>Bu araç, <strong>Ze'O</strong> tarafından geliştirildi.</em>
</p>