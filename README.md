<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Una galaxia de tulipanes para ti 🌷</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="container">
        <h1>Un jardín de tulipanes en la galaxia 🌌🌷</h1>
        <p class="mensaje">Para alguien que ilumina mis días de tantos colores como esta galaxia.</p>
        
        <div class="tulipanes-box">
            <!-- Aquí puedes poner imágenes de tulipanes coloridos o emojis -->
            <span class="tulipan">🌷</span>
            <span class="tulipan">🌸</span>
            <span class="tulipan">💛</span>
            <span class="tulipan">💜</span>
        </div>

        <button id="btnSorpresa">¡Haz clic para ver la magia!</button>
        <p id="textoOculto" class="oculto">Dicen que los tulipanes de colores significan alegría y buenos deseos. ¡Gracias por existir! ✨</p>
    </div>

    <!-- Música opcional de fondo -->
    <audio id="musica" src="TU_ENLACE_DE_AUDIO.mp3" loop></audio>

    <script src="script.js"></script>
</body>
</html>
body {
    background: radial-gradient(circle at center, #1b1b2f 0%, #0f0c1b 100%);
    color: #ffffff;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    text-align: center;
    height: 100vh;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
}

.container {
    background: rgba(255, 255, 255, 0.05);
    padding: 30px;
    border-radius: 20px;
    box-shadow: 0 0 20px rgba(255, 215, 0, 0.2);
    max-width: 400px;
    width: 90%;
    backdrop-filter: blur(5px);
}

h1 {
    font-size: 24px;
    color: #ffe600;
    text-shadow: 0 0 10px rgba(255, 230, 0, 0.5);
}

.mensaje {
    font-size: 16px;
    color: #e0e0e0;
    margin-bottom: 20px;
}

.tulipanes-box, .lirios-box {
    font-size: 40px;
    margin: 20px 0;
    display: flex;
    justify-content: space-around;
}

button {
    background: #ffcc00;
    color: #1b1b2f;
    border: none;
    padding: 10px 20px;
    font-size: 16px;
    font-weight: bold;
    border-radius: 25px;
    cursor: pointer;
    box-shadow: 0 0 10px #ffcc00;
    transition: 0.3s;
}

button:hover {
    background: #ffffff;
    box-shadow: 0 0 15px #ffffff;
}

.oculto {
    display: none;
    margin-top: 15px;
    font-size: 15px;
    color: #ff99c8;
    animation: fadeIn 1s ease-in-out;
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}
const btn = document.getElementById('btnSorpresa');
const textoOculto = document.getElementById('textoOculto');
const musica = document.getElementById('musica');

btn.addEventListener('click', () => {
    // Muestra el texto secreto
    textoOculto.style.display = 'block';
    btn.style.display = 'none'; // Oculta el botón al hacer clic

    // Intenta reproducir la música de fondo
    musica.play().catch(error => {
        console.log;
    });
});