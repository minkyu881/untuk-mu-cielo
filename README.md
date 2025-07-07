# untuk-mu-cielo   

slide pertama ini
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Buat Sayangku 💖</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      background-color: #fff0f5;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
      text-align: center;
    }
    h1 {
      font-size: 2em;
      color: #e91e63;
      margin-bottom: 20px;
    }
    .hidden {
      display: none;
    }
    button {
      padding: 12px 24px;
      background-color: #e91e63;
      color: #fff;
      border: none;
      border-radius: 25px;
      font-size: 1em;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    button:hover {
      background-color: #d81b60;
    }
  </style>
</head>
<body>

  <h1 id="text1">hai sayangku, pencet ini ya</h1>
  <button onclick="nextStep()">❤️ Klik di sini ❤️</button>

  <div id="step2" class="hidden">
    <h1>aku ada pesan buat kamu</h1>
    <a href="index.html">
      <button>Lihat Pesannya</button>
    </a>
  </div>

  <script>
    function nextStep() {
      document.getElementById("text1").style.display = "none";
      document.querySelector("button").style.display = "none";
      document.getElementById("step2").classList.remove("hidden");
    }
  </script>

</body>
</html>
 
slide kedua : 
`<img src="foto.png" alt="Foto berdua" />` di awal body (sebelum judul):

```html name=cielo.html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Untuk Cielo</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      background-color: #fffafa;
      font-family: 'Poppins', sans-serif;
      color: #333;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
      min-height: 100vh;
      text-align: center;
      overflow-x: hidden;
      padding: 40px 20px;
    }
    img {
      width: 90%;
      max-width: 400px;
      border-radius: 15px;
      margin-bottom: 30px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }
    h1 {
      font-size: 2.5em;
      font-weight: 600;
      margin-bottom: 20px;
      color: #ff4d6d;
    }
    p {
      font-size: 1em;
      max-width: 700px;
      font-weight: 300;
      color: #444;
      margin-bottom: 30px;
      line-height: 1.8;
      white-space: pre-wrap;
    }
    button {
      padding: 10px 25px;
      border: none;
      background: #ff4d6d;
      color: white;
      font-size: 1em;
      border-radius: 30px;
      cursor: pointer;
      transition: 0.3s ease;
    }
    button:hover { background: #e8435b; }

    .love {
      position: fixed;
      top: -20px;
      font-size: 20px;
      color: #ff4d6d;
      animation: fall 5s linear infinite;
      z-index: 100;
    }

    @keyframes fall {
      0% { transform: translateY(0) rotate(0deg); opacity: 1; }
      100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
    }
  </style>
</head>
<body>

  <img src="foto.png" alt="Foto berdua" />

  <h1>Untuk Cielo 💌</h1>
  <p>
bro—eh maksudnya, sayang

kadang aku masih ngga percaya bisa nemu pacar kayak kamu. tapi karna kamu tuh paket komplit pake telur, bisa bikin ketawa, tempat curhat, dan yang paling penting bisa ngertiin aku, bahkan pas aku lagi ngga ngerti diri sendiri.

terimakasih ya sayang udah tahan sama aku yang pendiam (cool), ganteng, dan sibuk ini. seriusan hari-hari biasa jadi luar biasa sejak ada kamu.

kamu tuh bukan cuma pacar, tapi juga sahabat, partner in crime, dan alarm hidup yang selalu nanyain "gimana harinya dan ingetin jangan begadang"

aku nggak janji bakal jadi cowok paling sempurna, tapi aku janji nggak akan ninggalin kamu. kita udah jalan sejauh ini, kamu pacar paling lucu dan menggemaskan yg pernah aku temuin.

Stay weird, stay mine.
  </p>

  <button onclick="alert('I choose you. Always. 💘')">iloveyou

  <script>
    const createLove = () => {
      const love = document.createElement('div');
      love.classList.add('love');
      love.innerText = '❤️';
      love.style.left = Math.random() * 100 + 'vw';
      love.style.fontSize = Math.random() * 20 + 10 + 'px';
      document.body.appendChild(love);
      setTimeout(() => { love.remove(); }, 5000);
    };
    setInterval(createLove, 300);
  </script>

</body>
</html>
```
