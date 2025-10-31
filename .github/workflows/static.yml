<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡Feliz Cumpleaños!</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #fce4ec, #f8bbd9);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 20px;
            color: #5d4037;
            overflow-x: hidden;
        }
        
        .screen {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            width: 100%;
            max-width: 600px;
            text-align: center;
        }
        
        #welcome-screen {
            z-index: 10;
        }
        
        #gift-screen {
            display: none;
        }
        
        .container {
            width: 100%;
            text-align: center;
            background-color: rgba(255, 224, 224, 0.85);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .container::before {
            content: "";
            position: absolute;
            top: -50px;
            left: -50px;
            width: 100px;
            height: 100px;
            background: rgba(255, 193, 7, 0.2);
            border-radius: 50%;
        }
        
        .container::after {
            content: "";
            position: absolute;
            bottom: -50px;
            right: -50px;
            width: 150px;
            height: 150px;
            background: rgba(233, 30, 99, 0.1);
            border-radius: 50%;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 30px;
            color: #e91e63;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
        }
        
        h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #7b1fa2;
        }
        
        .welcome-message {
            font-size: 1.5rem;
            margin-bottom: 30px;
            color: #5d4037;
        }
        
        .open-btn {
            padding: 15px 40px;
            font-size: 1.3rem;
            background: linear-gradient(to right, #e91e63, #ad1457);
            color: white;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        
        .open-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }
        
        .sunflower-container {
            margin: 20px auto;
            width: 250px;
            height: 350px;
            position: relative;
        }
        
        .stem {
            width: 12px;
            height: 200px;
            background: linear-gradient(to right, #2e7d32, #4caf50);
            margin: 0 auto;
            border-radius: 6px;
            position: relative;
            top: 150px;
            transform: scaleY(0);
            transform-origin: bottom;
        }
        
        .flower {
            width: 180px;
            height: 180px;
            position: relative;
            margin: 0 auto;
            top: -50px;
        }
        
        .center {
            width: 90px;
            height: 90px;
            background: radial-gradient(circle, #5d4037 0%, #3e2723 100%);
            border-radius: 50%;
            position: absolute;
            top: -35px;
            left: 45px;
            z-index: 10;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
            transform: scale(0);
        }
        
        .petal {
            width: 45px;
            height: 110px;
            background: linear-gradient(to bottom, #ffffff, #ecebea);
            border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
            position: absolute;
            top: -100px;
            left: 67.5px;
            transform-origin: 50% 100%;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
            transform: scale(0);
            z-index: 5;
        }
        
        .leaf {
            width: 0px;
            height: 50px;
            background: linear-gradient(to right, #2e7d32, #4caf50);
            border-radius: 0 50% 50% 0;
            position: absolute;
            top: 250px;
            left: calc(50% + 5px);
            transform: rotate(-20deg) scale(0);
            transform-origin: left center;
        }
        
        .leaf::before {
            content: "";
            position: absolute;
            width: 30px;
            height: 40px;
            background: linear-gradient(to left, #2e7d32, #4caf50);
            border-radius: 50% 0 0 50%;
            top: 2px;
            left: -40px;
            transform: rotate(10deg);
        }
        
        .drawing-line {
            stroke-dasharray: 1000;
            stroke-dashoffset: 1000;
            animation: draw 2s ease-in-out forwards;
        }
        
        @keyframes draw {
            to {
                stroke-dashoffset: 0;
            }
        }
        
        .message {
            margin: 30px 0;
            font-size: 1.5rem;
            color: #7b1fa2;
            font-weight: 600;
        }
        
        .buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        
        button {
            padding: 12px 30px;
            font-size: 1.2rem;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        
        #yesBtn {
            background: linear-gradient(to right, #e91e63, #ad1457);
            color: white;
        }
        
        #noBtn {
            background: linear-gradient(to right, #9c27b0, #7b1fa2);
            color: white;
        }
        
        button:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }
        
        button:active {
            transform: translateY(1px);
        }
        
        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background-color: #f44336;
            border-radius: 50%;
            animation: fall 5s linear infinite;
        }
        
        @keyframes fall {
            0% {
                transform: translateY(-100px) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(100vh) rotate(360deg);
                opacity: 0;
            }
        }
        
        @media (max-width: 500px) {
            h1 {
                font-size: 2rem;
            }
            
            h2 {
                font-size: 1.7rem;
            }
            
            .sunflower-container {
                width: 200px;
                height: 280px;
            }
            
            .flower {
                width: 140px;
                height: 140px;
            }
            
            .center {
                width: 70px;
                height: 70px;
                top: 35px;
                left: 35px;
            }
            
            .petal {
                width: 35px;
                height: 85px;
                top: 28px;
                left: 52.5px;
            }
            
            .stem {
                height: 150px;
                top: 130px;
            }
            
            .leaf {
                top: 230px;
            }
        }
    </style>
</head>
<body>
    <!-- Pantalla de bienvenida -->
    <div class="screen" id="welcome-screen">
        <div class="container">
            <h1>Este es tu regalito</h1>
            <h2>no te debo :P</h2>
            <p class="welcome-message">es sencillito pero espero te guste <br> Pd: sinceramente no creo que te guste el rosado pero como es color de mujer JASDKkj</p>
            <button class="open-btn" id="openBtn">Abrir</button>
        </div>
    </div>
    
    <!-- Pantalla del regalo -->
    <div class="screen" id="gift-screen">
        <div class="container">
            <h1>¡Feliz Cumpleaños!
                <br>
                espero que cumplas muchos años mas y que hoy tengas un bonito dia :D
            </h1>
            
            <div class="sunflower-container">
                <div class="stem" id="stem"></div>
                <div class="flower" id="flower">
                    <div class="center" id="center"></div>
                    <!-- Los pétalos se generarán con JavaScript -->
                </div>
                <div class="leaf" id="leaf"></div>
            </div>
            
            <div class="message">¿Quieres un tostón?</div>
            
            <div class="buttons">
                <button id="yesBtn">No</button>
                <button id="noBtn">Si</button>
            </div>
        </div>
    </div>

    <script>
        // Elementos de las pantallas
        const welcomeScreen = document.getElementById('welcome-screen');
        const giftScreen = document.getElementById('gift-screen');
        const openBtn = document.getElementById('openBtn');
        
        // Elementos del girasol
        const stem = document.getElementById('stem');
        const center = document.getElementById('center');
        const leaf = document.getElementById('leaf');
        const flower = document.getElementById('flower');
        
        // Función para cambiar de pantalla
        openBtn.addEventListener('click', function() {
            console.log('Botón Abrir clickeado');
            
            // Ocultar pantalla de bienvenida
            welcomeScreen.style.display = 'none';
            
            // Mostrar pantalla del regalo
            giftScreen.style.display = 'flex';
            
            // Iniciar animación del girasol
            drawSunflower();
        });
        
        // Función para dibujar el girasol gradualmente
        function drawSunflower() {
            // Limpiar pétalos existentes
            const existingPetals = flower.querySelectorAll('.petal');
            existingPetals.forEach(petal => petal.remove());
            
            // Resetear elementos del girasol
            stem.style.transform = 'scaleY(0)';
            center.style.transform = 'scale(0)';
            leaf.style.transform = 'rotate(-15deg) scale(0)';
            
            // Crear pétalos
            const petalCount = 16;
            const petals = [];
            
            for (let i = 0; i < petalCount; i++) {
                const petal = document.createElement('div');
                petal.className = 'petal';
                // Los pétalos deben rodear el centro correctamente
                petal.style.transform = `rotate(${i * (360 / petalCount)}deg) scale(0)`;
                flower.appendChild(petal);
                petals.push(petal);
            }
            
            // Animación secuencial mejorada - como dibujo real
            // 1. Tallo crece desde abajo (más lento, como dibujando)
            setTimeout(() => {
                stem.style.transition = 'transform 2s ease-out';
                stem.style.transform = 'scaleY(1)';
                
                // 2. Centro aparece con efecto de dibujo
                setTimeout(() => {
                    center.style.transition = 'transform 1.5s cubic-bezier(0.68, -0.55, 0.265, 1.55)';
                    center.style.transform = 'scale(1)';
                    
                    // 3. Pétalos aparecen en secuencia, como si los estuvieran dibujando
                    setTimeout(() => {
                        petals.forEach((petal, index) => {
                            setTimeout(() => {
                                petal.style.transition = 'transform 0.8s cubic-bezier(0.68, -0.55, 0.265, 1.55)';
                                petal.style.transform = `rotate(${index * (360 / petalCount)}deg) scale(1)`;
                                
                                // Efecto adicional: pequeño rebote al final
                                setTimeout(() => {
                                    petal.style.transition = 'transform 0.3s ease-out';
                                    petal.style.transform = `rotate(${index * (360 / petalCount)}deg) scale(1.05)`;
                                    setTimeout(() => {
                                        petal.style.transform = `rotate(${index * (360 / petalCount)}deg) scale(1)`;
                                    }, 300);
                                }, 800);
                            }, index * 150); // Espaciado entre pétalos
                        });
                        
                        // 4. Hojas aparecen al final con efecto de dibujo
                        setTimeout(() => {
                            leaf.style.transition = 'transform 1.2s cubic-bezier(0.68, -0.55, 0.265, 1.55)';
                            leaf.style.transform = 'rotate(-15deg) scale(1)';
                            
                            // Efecto de rebote para la hoja también
                            setTimeout(() => {
                                leaf.style.transition = 'transform 0.4s ease-out';
                                leaf.style.transform = 'rotate(-15deg) scale(1.1)';
                                setTimeout(() => {
                                    leaf.style.transform = 'rotate(-15deg) scale(1)';
                                }, 400);
                            }, 1200);
                            
                        }, petalCount * 150 + 500);
                        
                    }, 1000);
                }, 1000);
            }, 300);
        }
        
        // Crear confeti
        function createConfetti() {
            const colors = ['#e91e63', '#9c27b0', '#2196f3', '#4caf50', '#ffeb3b', '#ff9800'];
            
            for (let i = 0; i < 50; i++) {
                const confetti = document.createElement('div');
                confetti.className = 'confetti';
                confetti.style.left = Math.random() * 100 + 'vw';
                confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
                confetti.style.animationDelay = Math.random() * 5 + 's';
                confetti.style.width = Math.random() * 10 + 5 + 'px';
                confetti.style.height = confetti.style.width;
                document.body.appendChild(confetti);
            }
        }
        
        // Funciones para los botones
        document.getElementById('yesBtn').addEventListener('click', function() {
            alert('gracia a dio poq no tenia plata JDAKJKSAD. No mentira despues te doy tu toston :D');
            createConfetti();
        });
        
        document.getElementById('noBtn').addEventListener('click', function() {
            // Hacemos que el botón "No" se mueva cuando intenten hacer clic en él
            const noBtn = document.getElementById('noBtn');
            const container = document.querySelector('#gift-screen .container');
            const containerRect = container.getBoundingClientRect();
            
            // Calculamos una posición aleatoria dentro del contenedor
            const maxX = containerRect.width - noBtn.offsetWidth;
            const maxY = containerRect.height - noBtn.offsetHeight;
            
            const randomX = Math.floor(Math.random() * maxX);
            const randomY = Math.floor(Math.random() * maxY);
            
            noBtn.style.position = 'absolute';
            noBtn.style.left = randomX + 'px';
            noBtn.style.top = randomY + 'px';
            
            // Mensaje divertido
            const messages = [
                "¿Estas totalmente segura?",
                "Piensa tu respuesta bien",
                "SEGURA SEGURA??",
                "Piénsalo otra vez...",
                "Ten piedad a mi billetera :("
            ];
            
            const randomMessage = messages[Math.floor(Math.random() * messages.length)];
            document.querySelector('.message').textContent = randomMessage;
        });
        
        // Inicialización
        console.log('Aplicación cargada correctamente');
    </script>
</body>
</html>
