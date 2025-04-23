
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Surat Cinta Untukmu</title>
    <style>
        body { margin: 0; font-family: 'Segoe UI', sans-serif; background: #ffe6f0; color: #333; overflow: hidden; }
        .slide { width: 100vw; height: 100vh; display: none; flex-direction: column; justify-content: center; align-items: center; padding: 40px; text-align: center; }
        .slide.active { display: flex; }
        h1 { color: #e60073; font-size: 2em; margin-bottom: 20px; }
        p { font-size: 1.2em; max-width: 600px; }
        .next-btn { margin-top: 30px; padding: 10px 20px; background: #e60073; color: white; border: none; border-radius: 10px; cursor: pointer; font-size: 1em; }
        .emoji { font-size: 4em; margin: 20px 0; }
    </style>
</head>
<body>

<div class="slide active">
    <h1>Slide 1: Awal Cerita</h1>
    <div class="emoji">✨</div>
    <p>Kita mungkin hanya dua manusia biasa, tapi sejak aku mengenalmu, semuanya terasa luar biasa. Dunia yang datar jadi penuh warna.</p>
    <button class="next-btn">Lanjut</button>
</div>

<div class="slide">
    <h1>Slide 2: Saat Bersamamu</h1>
    <div class="emoji">⏳</div>
    <p>Tawa kecilmu, caramu menyebut namaku, bahkan diam kita… semuanya jadi momen yang ingin aku simpan selamanya.</p>
    <button class="next-btn">Lanjut</button>
</div>

<div class="slide">
    <h1>Slide 3: Terima Kasih</h1>
    <div class="emoji">❤️</div>
    <p>Terima kasih sudah hadir di hidupku. Kamu bukan hanya pacar, kamu adalah rumah yang selalu ingin aku pulang.</p>
    <button class="next-btn">Lanjut</button>
</div>

<div class="slide">
    <h1>Slide 4: Untuk Hari Esok</h1>
    <div class="emoji">🌅</div>
    <p>Aku tak tahu pasti ke mana hidup membawa kita. Tapi satu yang aku tahu, aku ingin kamu tetap di sisiku — esok, lusa, dan selamanya.</p>
    <button class="next-btn">Lanjut</button>
</div>

<div class="slide">
    <h1>Slide 5: Dari Si Paling Cinta</h1>
    <div class="emoji">‍‍❤️‍‍</div>
    <p>Ini bukan surat biasa. Ini adalah sebagian kecil dari rasa sayangku buat kamu. Teruslah bersinar, cintaku.</p>
</div>

<script>
    const slides = document.querySelectorAll('.slide');
    const buttons = document.querySelectorAll('.next-btn');
    let current = 0;

    buttons.forEach(btn => {
        btn.addEventListener('click', () => {
            slides[current].classList.remove('active');
            current++;
            if (current < slides.length) {
                slides[current].classList.add('active');
            }
        });
    });
</script>

</body>
</html>
