# for-u
justtt for u for realll
<!DOCTYPE html><html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Buat Kamu 💖</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      font-family: 'Segoe UI', sans-serif;
    }
    .card {
      background: white;
      padding: 30px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
      max-width: 320px;
      animation: fadeIn 1.2s ease;
    }
    h1 {
      margin-bottom: 10px;
      color: #ff5e78;
    }
    p {
      color: #555;
      font-size: 16px;
    }
    button {
      margin: 10px;
      padding: 10px 20px;
      border: none;
      border-radius: 25px;
      font-size: 16px;
      cursor: pointer;
      transition: 0.3s;
    }
    .yes {
      background: #ff5e78;
      color: white;
    }
    .yes:hover {
      background: #ff2f55;
    }
    .no {
      background: #ddd;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.9); }
      to { opacity: 1; transform: scale(1); }
    }
  </style>
</head>
<body>
  <div class="card" id="card">
    <h1>Hai Kamu 💕</h1>
    <p>Aku udah mikir lama…</p>
    <p><strong>Mau gak jadi orang spesial di hidup aku?</strong></p>
    <button class="yes" onclick="jawabYa()">Iya 💖</button>
    <button class="no" onmouseover="kabur()">Enggak 🙃</button>
  </div>  <script>
    function jawabYa() {
      document.getElementById('card').innerHTML = `
        <h1>Yay! 🥰</h1>
        <p>Mulai sekarang…</p>
        <p><strong>Kamu milik aku ❤️</strong></p>
      `;
    }

    function kabur() {
      const btn = document.querySelector('.no');
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 200 - 100;
      btn.style.transform = `translate(${x}px, ${y}px)`;
    }
  </script></body>
</html>
