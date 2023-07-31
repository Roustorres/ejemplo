<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Corazón Latiendo</title>
    <link rel="stylesheet" href="dante.css">
</head>
<body>
    <div class="heart-container">
        <svg class="heart" viewBox="0 0 32 29.6">
            <path d="M16 29.6C15.1 29.6 14.1 29.1 13.4 28.4L2.4 17.4C-0.7 14.3 -0.7 9.8 2.4 6.7C5.5 3.6 10 3.6 13.1 6.7L16 9L18.9 6.7C22 3.6 26.5 3.6 29.6 6.7C32.7 9.8 32.7 14.3 29.6 17.4L18.6 28.4C17.9 29.1 16.9 29.6 16 29.6Z" fill="red" />
        </svg>
    </div>
    <div class="name">Cristhian Dante</div>
    <div class="love">TE AMO</div>
  
</body>
</html>
body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    background-color: black; /* Fondo verde para toda la página */
    font-family: Arial, sans-serif;
}

.heart-container {
    position: relative;
    animation: heartbeat 1s infinite;
}

.heart {
    width: 100px;
    height: 100px;
    filter: drop-shadow(0 0 2px rgba(255, 255, 255, 0.6)) brightness(120%); /* Sombra un poquito más ancha y brillo aumentado en todo el corazón */
}

.name {
    font-size: 24px;
    margin-top: 10px;
    color: #B52B55; /* Cambiamos el color a azul */
    text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.6);
    animation: colorChange 5s infinite;
}

.love {
    font-size: 24px;
    color: #B52B55; /* Cambiamos el color a azul */
    text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.6);
    animation: colorChange 5s infinite;
}

@keyframes heartbeat {
    0%, 100% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.1);
    }
}

@keyframes colorChange {
    0% {
        color: #B52B55; /* Cambiamos el color a azul */
    }
    50% {
        color: rgba(255, 255, 255, 0.6);
    }
    100% {
        color: #B52B55; /* Cambiamos el color a azul */
    }
}
