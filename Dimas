<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Undangan Pernikahan Yanto & Dimas</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/animejs@3.2.1/lib/anime.min.js"></script>
  <style>
    body {
      background: linear-gradient(to bottom, #fffdf9, #fff4db);
      color: #4b3b2f;
      font-family: 'Cormorant Garamond', serif;
      overflow: hidden;
    }
    .slide {
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      opacity: 0;
      transition: opacity 1s ease;
    }
    .slide.active {
      opacity: 1;
    }
    .btn {
      background: linear-gradient(to right, #b98b36, #d4af37);
      color: white;
      padding: 10px 20px;
      border-radius: 8px;
      font-weight: 600;
      transition: 0.3s;
    }
    .btn:hover {
      background: linear-gradient(to right, #d4af37, #b98b36);
    }
    .nav-btn {
      color: #b98b36;
      font-weight: bold;
      cursor: pointer;
      margin: 10px;
    }
  </style>
</head>
<body class="relative w-screen h-screen flex items-center justify-center">

  <div id="slides" class="w-full h-full text-center relative">
    <!-- Slide 1 -->
    <div class="slide active" id="slide1">
      <div>
        <h1 class="text-3xl text-yellow-700 mb-2">Undangan Pernikahan</h1>
        <h2 class="text-5xl font-bold text-gray-900 mb-4">Yanto & Dimas</h2>
        <p class="italic">Minggu, 7 Februari 2027</p>
        <p>Pondok Bambu Kalibaru, Banyuwangi</p>
      </div>
    </div>

    <!-- Slide 2 -->
    <div class="slide" id="slide2">
      <div class="max-w-xl">
        <p class="italic text-lg">
          “Dan di antara tanda-tanda (kebesaran)-Nya ialah Dia menciptakan
          untukmu pasangan-pasangan dari jenismu sendiri, supaya kamu
          cenderung dan merasa tenteram kepadanya, dan dijadikan-Nya di
          antaramu rasa kasih dan sayang.”
        </p>
        <p class="mt-4 font-semibold text-yellow-700">(QS. Ar-Rum: 21)</p>
      </div>
    </div>

    <!-- Slide 3 -->
    <div class="slide" id="slide3">
      <div>
        <h3 class="text-2xl font-semibold text-yellow-700 mb-2">Detail Acara</h3>
        <p>Minggu, 7 Februari 2027<br>Pukul 15:00 WIB – selesai</p>
        <p class="mt-3 font-semibold">Tempat:</p>
        <p>Pondok Bambu Kalibaru, Banyuwangi, Jawa Timur</p>
      </div>
    </div>

    <!-- Slide 4 -->
    <div class="slide" id="slide4">
      <div>
        <h3 class="text-2xl font-semibold text-yellow-700 mb-2">Lokasi Acara</h3>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3944.651707002159!2d114.150!3d-8.266!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2dd166b3c50a8c33%3A0x6a3f73d3edc5dc14!2sKalibaru%2C%20Banyuwangi!5e0!3m2!1sen!2sid!4v0000000000"
          width="100%" height="250" class="rounded-xl shadow border border-yellow-200"
          allowfullscreen loading="lazy"></iframe>
      </div>
    </div>

    <!-- Slide 5 -->
    <div class="slide" id="slide5">
      <div class="max-w-md mx-auto">
        <h3 class="text-2xl font-semibold text-yellow-700 mb-3">Konfirmasi Kehadiran</h3>
        <form action="https://formsubmit.co/ytkedua929@gmail.com" method="POST" class="space-y-3">
          <input type="text" name="Nama" placeholder="Nama Anda" required class="w-full border p-2 rounded">
          <select name="Kehadiran" required class="w-full border p-2 rounded">
            <option value="">Pilih Kehadiran</option>
            <option value="Hadir">Hadir</option>
            <option value="Tidak Hadir">Tidak Hadir</option>
          </select>
          <button type="submit" class="btn w-full">Kirim</button>
        </form>
      </div>
    </div>

    <!-- Slide 6 -->
    <div class="slide" id="slide6">
      <div>
        <p class="italic mb-2 text-gray-700">Kehadiran dan doa restu Anda merupakan kebahagiaan bagi kami.</p>
        <h3 class="text-3xl font-semibold text-yellow-700">Yanto & Dimas</h3>
      </div>
    </div>
  </div>

  <!-- Navigation -->
  <div class="absolute bottom-6 w-full flex justify-center gap-10 text-lg">
    <span id="prevBtn" class="nav-btn">‹ Sebelumnya</span>
    <span id="nextBtn" class="nav-btn">Selanjutnya ›</span>
  </div>

  <script>
    const slides = document.querySelectorAll(".slide");
    let current = 0;

    const showSlide = (index) => {
      slides.forEach((slide, i) => {
        slide.classList.toggle("active", i === index);
      });
      anime({
        targets: slides[index],
        opacity: [0, 1],
        translateY: [50, 0],
        duration: 800,
        easing: 'easeOutQuad'
      });
    };

    document.getElementById("nextBtn").addEventListener("click", () => {
      current = (current + 1) % slides.length;
      showSlide(current);
    });

    document.getElementById("prevBtn").addEventListener("click", () => {
      current = (current - 1 + slides.length) % slides.length;
      showSlide(current);
    });
  </script>

</body>
</html>
