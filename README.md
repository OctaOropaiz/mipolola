<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Para Mi Amor</title>
    <style>
        body {
            background-color: #000000;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            overflow: hidden;
            font-family: 'Courier New', Courier, monospace;
        }
        svg {
            width: 95%;
            max-width: 460px;
            height: auto;
        }
        path {
            stroke-dasharray: 1600;
            stroke-dashoffset: 1600;
            animation: draw 6.8s ease-in-out forwards;
        }
        .tallo { stroke: #00b451; stroke-width: 4; fill: none; stroke-linecap: round; animation-delay: 0s; }
        .hojas { stroke: #00b451; stroke-width: 4; fill: none; stroke-linecap: round; animation-delay: 1.5s; }
        .rosa-capullo { stroke: #e61a1a; stroke-width: 4.5; fill: none; stroke-linecap: round; animation-delay: 2.8s; }
        .rosa-detalles { stroke: #e61a1a; stroke-width: 4.5; fill: none; stroke-linecap: round; animation-delay: 3.8s; }
        /* El nuevo corazón con trazos menos curvos basados en tu dibujo */
        .corazon-boceto { stroke: #ff3333; stroke-width: 4.5; fill: none; stroke-linecap: round; animation-delay: 5.5s; }
        
        .mensaje {
            margin-top: 15px;
            color: #ff3333;
            font-size: 1.2rem;
            opacity: 0;
            animation: fadeIn 1.5s 7.5s forwards;
            text-align: center;
            text-shadow: 0 0 8px rgba(255, 51, 51, 0.6);
        }

        @keyframes draw {
            to { stroke-dashoffset: 0; }
        }
        @keyframes fadeIn {
            to { opacity: 1; }
        }
    </style>
</head>
<body>

    <svg viewBox="0 0 200 240">
        <!-- Tallo central curvo -->
        <path class="tallo" d="M 97,125 Q 94,170 94,220 C 94,225 80,215 70,205" />
        
        <!-- Dos hojas redondeadas -->
        <path class="hojas" d="M 95,148 Q 120,135 118,145 Q 115,150 95,152" />
        <path class="hojas" d="M 94,165 Q 70,150 80,165 Q 88,172 94,168" />
        
        <!-- Capullo exterior de la rosa -->
        <path class="rosa-capullo" d="M 76,82 C 70,95 75,120 100,125 C 118,122 120,95 114,82 C 108,72 88,72 76,82 Z" />
        
        <!-- Detalles internos -->
        <path class="rosa-detalles" d="M 80,82 C 86,95 106,115 116,92" />
        <path class="rosa-detalles" d="M 112,85 C 100,98 84,105 84,115" />
        <path class="rosa-detalles" d="M 84,82 Q 100,75 110,82" />
        <path class="rosa-detalles" d="M 90,84 Q 100,90 106,84" />
        
        <!-- Corazón calcado de tu última foto: orejas más planas y caídas más rectas -->
        <path class="corazon-boceto" d="M 100,52 C 75,22 45,28 25,65 C 5,115 35,160 88,225 L 100,236 L 112,225 C 165,160 195,115 175,65 C 155,28 125,22 100,52 Z" />
    </svg>

    <div class="mensaje">
        &lt;code&gt;<br>
        Te amo con todo mi ser mi estrellita lindota!<br>
        &lt;/code&gt;
    </div>

</body>
</html>
