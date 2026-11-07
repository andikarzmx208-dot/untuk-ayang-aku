<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Maaf Untuk Syakira ❤️</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    min-height: 100vh;
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(135deg, #ff758c, #ffb6c1, #ffc3a0);
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    padding: 20px;
}

.container {
    background: rgba(255,255,255,0.92);
    max-width: 420px;
    width: 100%;
    padding: 35px 25px;
    border-radius: 25px;
    text-align: center;
    box-shadow: 0 15px 40px rgba(0,0,0,0.15);
    position: relative;
    z-index: 2;
}

.heart {
    font-size: 65px;
    animation: beat 1s infinite;
}

@keyframes beat {
    50% { transform: scale(1.2); }
}

h1 {
    color: #e84370;
    margin: 15px 0;
    font-size: 27px;
}

.name {
    color: #ff4f81;
    font-weight: bold;
    font-size: 20px;
    margin-bottom: 15px;
}

p {
    color: #555;
    line-height: 1.8;
    font-size: 14px;
}

button {
    border: none;
    background: linear-gradient(135deg, #ff4f81, #ff758c);
    color: white;
    padding: 13px 25px;
    border-radius: 30px;
    margin-top: 25px;
    font-size: 15px;
    cursor: pointer;
    transition: 0.3s;
}

button:hover {
    transform: scale(1.07);
}

#pesan {
    display: none;
    margin-top: 25px;
    animation: muncul 1s;
}

@keyframes muncul {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.footer {
    margin-top: 25px;
    color: #999;
    font-size: 12px;
}

.falling-heart {
    position: fixed;
    top: -30px;
    animation: jatuh linear forwards;
    pointer-events: none;
    z-index: 1;
}

@keyframes jatuh {
    to {
        transform: translateY(110vh) rotate(360deg);
        opacity: 0;
    }
}
</style>
</head>

<body>

<div class="container">

    <div class="heart">❤️</div>

    <h1>AKU MINTA MAAF YAAAA</h1>

    <div class="name">
        TAYANG AKUUU Syakira Nuryasa Kusuma
    </div>

    <p>
        SAYANGGGGGG INI AKUUUU🥹🥹🥹
        <br> ini aku yang selalu kangen sama kamuu
        selalu mikirin kamu, selalu overthinking tentang kamu, dan selalu cerewet sama kamu.
    </p>

    <button onclick="bukaPesan()">
        Buka Pesan ❤️
    </button>

    <div id="pesan">

        <h2 style="color:#e84370; margin-bottom:15px;">
            Untuk Syakira ❤️
        </h2>

        <p>
            cayangg... <br>
            aku sadar aku banyak salah sama kamu, aku belum layak untuk kanu
            <br><br>
            Aku selalu saja buat salah karena aku yang terlalu bodoh
            aku selalu buat mood kamu berantakan, buat kamu marah
            <br><br>
            Aku selalu sayang samaa kamu tayangg, aku selalu mikirin kamu,
            aku selalu kangen kamu, aku selalu overthinking tentang kamu,
            aku gamau kehilangan kamuu, aku gamau kamu pergii
            <br><br>
            Terima kasih sudah membaca pesan ini.
            Maaf ya, tayang aku tercinta. ❤️
        </p>

        <h3 style="color:#ff4f81; margin-top:20px;">
            aku minta maaf❤️
        </h3>

    </div>

    <div class="footer">
        Made with ❤️ khusus untuk Syakira
    </div>

</div>

<script>
function bukaPesan() {
    const pesan = document.getElementById("pesan");

    pesan.style.display = "block";

    document.querySelector("button").style.display = "none";
}

function buatHati() {
    const hati = document.createElement("div");

    hati.className = "falling-heart";
    hati.innerHTML = ["❤️", "💕", "💗", "💖"][
        Math.floor(Math.random() * 4)
    ];

    hati.style.left = Math.random() * 100 + "vw";
    hati.style.fontSize = (15 + Math.random() * 20) + "px";
    hati.style.animationDuration = (3 + Math.random() * 4) + "s";

    document.body.appendChild(hati);

    setTimeout(() => hati.remove(), 7000);
}

setInterval(buatHati, 400);
</script>

</body>
</html>
