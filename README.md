<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Главная страница</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #1a1a1a;
            color: white;
            font-family: Arial, sans-serif;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }

        nav {
            background-color: #333;
            padding: 1rem;
            text-align: center;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 1.5rem;
            font-size: 1.1rem;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #00ff88;
        }

        .container {
            flex: 1;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 2rem;
        }

        .main-image {
            border: 3px solid white;
            border-radius: 10px;
            transition: transform 0.3s;
            max-width: 90%;
            height: auto;
        }

        .main-image:hover {
            transform: scale(1.05);
            cursor: pointer;
        }
    </style>
</head>
<body>
    <!-- Меню -->
    <nav>
        <a href="#main">Основное</a>
        <a href="#about">О нас</a>
        <a href="#order">Заказать</a>
    </nav>

    <!-- Основной контент -->
    <div class="container">
        <a href="https://example.com" target="_blank">
            <img 
                src="images/main-image.jpg" 
                alt="Основное изображение" 
                class="main-image"
            >
        </a>
    </div>
</body>
</html>
