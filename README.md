# birthday---surprise-
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ucapan Ulang Tahun untuk Crush</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to right, #ff9a9e, #fecfef);
            color: white;
            text-align: center;
            padding: 50px;
            margin: 0;
        }
        h1 {
            font-size: 3em;
            margin-bottom: 20px;
        }
        p {
            font-size: 1.5em;
            margin-bottom: 30px;
        }
        img {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            margin-bottom: 20px;
            border: 5px solid white;
        }
        button {
            background: #ff6b6b;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2em;
            cursor: pointer;
            border-radius: 10px;
            transition: background 0.3s;
        }
        button:hover {
            background: #ff5252;
        }
        #surprise {
            display: none;
            font-size: 2em;
            color: yellow;
            margin-top: 20px;
        }
        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background: red;
            animation: fall 3s linear infinite;
        }
        @keyframes fall {
            to {
                transform: translateY(100vh);
            }
        }
    </style>
</head>
<body>
    <h1>Selamat Ulang Tahun, [Nama Crush]!</h1>
    <img src="placeholder.jpg" alt="Foto Crush"> <!-- Ganti 'placeholder.jpg' dengan URL foto crush kamu -->
    <p>Hari ini adalah hari spesialmu! Semoga tahun ini penuh kebahagiaan, cinta, dan impian yang tercapai. Kamu adalah orang yang luar biasa, dan aku berharap kita bisa lebih dekat lagi. 😊</p>
    <button onclick="showSurprise()">Klik untuk Kejutan!</button>
    <div id="surprise">🎉 Selamat! Kamu mendapatkan kejutan virtual: Sebuah pelukan hangat dan harapan terbaik dari aku! 🎂</div>

    <script>
        function showSurprise() {
            document.getElementById('surprise').style.display = 'block';
            // Tambahkan confetti sederhana
            for (let i = 0; i < 50; i++) {
                let confetti = document.createElement('div');
                confetti.className = 'confetti';
                confetti.style.left = Math.random() * 100 + 'vw';
                confetti.style.animationDelay = Math.random() * 3 + 's';
                document.body.appendChild(confetti);
                setTimeout(() => confetti.remove(), 3000);
            }
        }
    </script>
</body>
</html>
