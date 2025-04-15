< html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Karadeniz İklimi</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #f0f0f0; }
    header { background: #34495e; padding: 20px; text-align: center; color: white; }
    nav { background: #2c3e50; display: flex; justify-content: center; }
    nav a { color: white; padding: 15px 20px; text-decoration: none; }
    nav a:hover { background: #1abc9c; }
    section { padding: 20px; display: none; }
    section.active { display: block; background: white; margin: 20px; border-radius: 10px; }
    img { width: 300px; margin: 10px; border-radius: 8px; }
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
  <img src="karadeniz1.jpg" alt="Karadeniz İklimi 1">
  <img src="karadeniz2.jpg" alt="Karadeniz İklimi 2">
</section>

<section id="bitki">
  <h2>Karadeniz İkliminde Bitki Türleri</h2>
  <p>Yoğun yağışlar ve yüksek nem, Karadeniz kıyılarında zengin bir bitki örtüsünün oluşmasına neden olmuştur. Kızılçam, kayın, meşe, ladin, gürgen gibi ağaç türleri sıkça görülür. Ormanlar çok gürdür ve yer yer orman altı florası da oldukça çeşitlidir. Ayrıca fındık, çay ve kivi gibi ekonomik bitkiler de bu bölgede yetiştirilir.</p>
  <img src="karadeniz_bitki1.jpg" alt="Karadeniz Bitki 1">
  <img src="karadeniz_bitki2.jpg" alt="Karadeniz Bitki 2">
</section>

<section id="hayvan">
  <h2>Karadeniz İkliminde Hayvan Türleri</h2>
  <p>Karadeniz ormanlarında yaşayan hayvanlar çeşitlidir. Ayı, geyik, karaca, sansar, porsuk gibi memeliler; ağaçkakan, atmaca, baykuş gibi kuş türleri yaygındır. Yüksek nemli ve yeşil alanlar, özellikle kuşlar için ideal yaşam alanıdır. Akarsu kenarlarında su samuru gibi nadir türler de gözlemlenebilir.</p>
  <img src="karadeniz_hayvan1.jpg" alt="Karadeniz Hayvan 1">
  <img src="karadeniz_hayvan2.jpg" alt="Karadeniz Hayvan 2">
</section>

<section id="foto">
  <h2>Tüm Fotoğraflar</h2>
  <img src="karadeniz1.jpg" alt="Karadeniz İklim">
  <img src="karadeniz2.jpg" alt="Karadeniz İklim 2">
  <img src="karadeniz_bitki1.jpg" alt="Bitki 1">
  <img src="karadeniz_bitki2.jpg" alt="Bitki 2">
  <img src="karadeniz_hayvan1.jpg" alt="Hayvan 1">
  <img src="karadeniz_hayvan2.jpg" alt="Hayvan 2">
</section>

<script>
  function showSection(id) {
    document.querySelectorAll('section').forEach(section => {
      section.classList.remove('active');
    });
    document.getElementById(id).classList.add('active');
  }
</script>

</body>
</html>
