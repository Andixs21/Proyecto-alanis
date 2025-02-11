<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Alanis</title>
    <style>
        body {
            background-image: url('https://github.com/Andixs21/Proyecto-alanis/blob/main/premium_photo-1671974489983-083171c0215e.jpeg?raw=true');
            background-size: cover;
            background-attachment: fixed;
            text-align: center;
            font-family: Arial, sans-serif;
            color: white;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            margin: auto;
            background: rgba(255, 182, 193, 0.8);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        h1, h2, p {
            margin-bottom: 15px;
        }
        h1 {
            font-size: 2.5em;
            color: #ff69b4;
        }
        p {
            font-size: 1.2em;
        }
        button {
            padding: 10px 20px;
            font-size: 1.2em;
            background-color: #ff4d4d;
            color: white;
            border: none;
            border-radius: 10px;
            cursor: pointer;
        }
        button:hover {
            background-color: #ff1a1a;
        }
        .hidden {
            display: none;
        }
        .images img {
            width: 100%;
            border-radius: 15px;
            margin-bottom: 15px;
            max-width: 400px;
        }
        .corner-text {
            font-size: 0.9em;
            color: #ffd700;
        }
        .tulip-animation {
            animation: growTulips 3s ease-in-out;
        }
        @keyframes growTulips {
            0% { transform: scale(0.5); opacity: 0; }
            100% { transform: scale(1); opacity: 1; }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Querida Alanis</h1>
        <p>Esto es algo especial hecho para ti por este próximo San Valentín, queriendo pedirte algo, con mucho amor Andi.</p>
        <button onclick="mostrarSeccion(1)">Siguiente</button>
    </div>

    <div id="seccion1" class="container hidden">
        <div class="images">
            <img src="https://raw.githubusercontent.com/Andixs21/Presentaci-n-para-alanis/ec92ba58334645f61c57e1cc9631c0608a64a744/Imagen%20de%20WhatsApp%202025-02-02%20a%20las%2014.02.58_0f69acd4.jpg" alt="Imagen 1">
            <img src="https://raw.githubusercontent.com/Andixs21/Presentaci-n-para-alanis/ec92ba58334645f61c57e1cc9631c0608a64a744/Imagen%20de%20WhatsApp%202025-02-02%20a%20las%2014.02.58_a019493d.jpg" alt="Imagen 2">
        </div>
        <p>Pronto serán 2 grandiosos años de nuestra hermosa relación y serán muchos más a tu lado felizmente.</p>
        <button onclick="mostrarSeccion(2)">Siguiente</button>
    </div>

    <div id="seccion2" class="container hidden">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSNbVyF70gJwdY6H0FpceiPJzFGo63GJqK-bg&s" 
             alt="Pompurin" 
             width="300">
        <h2 class="tulip-animation">¿Quieres ser mi San Valentín?</h2>
        <div>
            <button onclick="mostrarSeccion(3)">Sí</button>
            <button onclick="mostrarSeccion(3)">No (Sí)</button>
        </div>
    </div>

    <div id="seccion3" class="container hidden">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRlldBVzZ-VHW5esB7cwF7mazvILYYSQ9m66Q&s" 
             alt="Pompurin y Macaroon" 
             width="300">
        <p>Gracias por ser mi compañera en esta vida y por permitirme pasar contigo este San Valentín.</p>
        <p class="corner-text">
            Pdta.: <span class="resaltado">Así es</span>, no acepto un no por respuesta te amo JAJAJAJA.
        </p>
        <button onclick="mostrarSeccion(4)">Siguiente</button>
    </div>

    <div id="seccion4" class="container hidden">
        <img src="https://raw.githubusercontent.com/Andixs21/Presentaci-n-para-alanis/ec92ba58334645f61c57e1cc9631c0608a64a744/Imagen%20de%20WhatsApp%202025-02-02%20a%20las%2014.02.58_c6c158d9.jpg" 
             alt="Imagen Especial" style="max-width: 100%; height: auto;">
        <p>Gracias por todos estos momentos a tu lado, ya sean tristes, felices, emocionantes, incómodos, amorosos.</p>
        <button onclick="mostrarSeccion(5)">Final</button>
    </div>

    <div id="seccion5" class="container hidden">
        <p>Gracias por tu atención y aceptar mis sentimientos con esta presentación. Te amo mucho, mucho, mucho Alanis.</p>
        <p style="margin-top: 20px;">Atte.: Andixon, persona que te ama mucho.</p>
    </div>

    <script>
        function mostrarSeccion(seccion) {
            document.querySelectorAll('.container').forEach(div => div.classList.add('hidden'));
            document.getElementById(`seccion${seccion}`).classList.remove('hidden');
        }
    </script>
</body>
</html>
