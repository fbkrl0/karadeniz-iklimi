<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Karadeniz İklimi</title>
  <style>
    body { 
        font-family: 'Arial', sans-serif; 
        margin: 0; 
        padding: 0; 
        background: #f4f8fb; 
        color: #34495e;
        line-height: 1.6;
    }

    header { 
        background: #1abc9c; 
        padding: 20px; 
        text-align: center; 
        color: white; 
        border-bottom: 5px solid #16a085;
    }

    nav { 
        background: #34495e; 
        display: flex; 
        justify-content: center; 
        padding: 10px 0;
    }

    nav a { 
        color: white; 
        padding: 15px 25px; 
        text-decoration: none; 
        font-size: 18px;
        font-weight: bold; 
        transition: background 0.3s ease;
        border-radius: 5px;
        margin: 0 10px;
    }

    nav a:hover { 
        background: #16a085; 
    }

    section { 
        padding: 20px; 
        margin: 20px;
        background: white; 
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); 
        border-radius: 8px;
        display: none; /* Sekmelerin başlangıçta gizli olması için */
    }

    section.active { 
        display: block; /* Aktif sekme gösterilecek */
    }

    h2 { 
        font-size: 24px; 
        color: #1abc9c;
        text-align: center;
        margin-bottom: 20px;
    }

    p {
        font-size: 16px;
        text-align: justify;
    }

    .image-container {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 15px;
        margin-top: 20px;
    }

    img { 
        width: 100%;
        max-width: 350px;
        border-radius: 8px;
    }

  </style>
</head>
<body>

<header>
  <h1>Karadeniz İklimi</h1>
</header>

<nav>
  <a href="#" onclick="showSection('iklim')">İklim Özellikleri</a>
  <a href="#" onclick="showSection('bitki')">Bitki Türleri</a>
  <a href="#" onclick="showSection('hayvan')">Hayvan Türleri</a>
  <a href="#" onclick="showSection('foto')">Fotoğraflar</a>
</nav>

<section id="iklim" class="active">
  <h2>Karadeniz İklimi Özellikleri</h2>
  <p>Karadeniz iklimi, Türkiye'nin Karadeniz kıyılarında etkili olan nemli ve ılıman bir iklim tipidir. Yıl boyunca düzenli yağış alır, bu nedenle kurak bir dönem yaşanmaz. Yazlar serin, kışlar ılımandır. Yıllık sıcaklık farkı düşüktür. En belirgin özelliği yıl boyu yüksek nem oranıdır.</p>
  <div class="image-container">
    <img src="karadeniz1.jpg" alt="Karadeniz İklimi 1">
    <img src="karadeniz2.jpg" alt="Karadeniz İklimi 2">
  </div>
</section>

<section id="bitki">
  <h2>Karadeniz İkliminde Bitki Türleri</h2>
  <p>Yoğun yağışlar ve yüksek nem, Karadeniz kıyılarında zengin bir bitki örtüsünün oluşmasına neden olmuştur. Kızılçam, kayın, meşe, ladin, gürgen gibi ağaç türleri sıkça görülür. Ormanlar çok gürdür ve yer yer orman altı florası da oldukça çeşitlidir. Ayrıca fındık, çay ve kivi gibi ekonomik bitkiler de bu bölgede yetiştirilir.</p>
  <div class="image-container">
    <img src="karadeniz_bitki1.jpg" alt="Karadeniz Bitki 1">
    <img src="karadeniz_bitki2.jpg" alt="Karadeniz Bitki 2">
  </div>
</section>

<section id="hayvan">
  <h2>Karadeniz İkliminde Hayvan Türleri</h2>
  <p>Karadeniz ormanlarında yaşayan hayvanlar çeşitlidir. Ayı, geyik, karaca, sansar, porsuk gibi memeliler; ağaçkakan, atmaca, baykuş gibi kuş türleri yaygındır. Yüksek nemli ve yeşil alanlar, özellikle kuşlar için ideal yaşam alanıdır. Akarsu kenarlarında su samuru gibi nadir türler de gözlemlenebilir.</p>
  <div class="image-container">
    <img src="karadeniz_hayvan1.jpg" alt="Karadeniz Hayvan 1">
    <img src="karadeniz_hayvan2.jpg" alt="Karadeniz Hayvan 2">
  </div>
</section>

<section id="foto">
  <h2>Tüm Fotoğraflar</h2>
  <div class="image-container">
    <img src="karadeniz1.jpg" alt="Karadeniz İklim">
    <img src="karadeniz2.jpg" alt="Karadeniz İklim 2">
    <img src="karadeniz_bitki1.jpg" alt="Bitki 1">
    <img src="karadeniz_bitki2.jpg" alt="Bitki 2">
    <img src="karadeniz_hayvan1.jpg" alt="Hayvan 1">
    <img src="karadeniz_hayvan2.jpg" alt="Hayvan 2">
  </div>
</section>

<script>
  function showSection(id) {
    // Tüm section'ları gizle
    document.querySelectorAll('section').forEach(section => {
      section.classList.remove('active');
    });
    // Seçilen section'ı göster
    document.getElementById(id).classList.add('active');
  }
</script>

</body>
</html>
