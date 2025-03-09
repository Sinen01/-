ваша_папка/
├── index.html
├── style.css
└── script.js

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мой Первый Сайт</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Главная</a></li>
                <li><a href="#about">О нас</a></li>
                <li><a href="#contact">Контакты</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home">
            <h1>Добро пожаловать!</h1>
            <p>Это мой первый веб-сайт</p>
            <button id="changeColorBtn">Изменить цвет</button>
        </section>

        <section id="about">
            <h2>О нас</h2>
            <p>Мы учимся создавать веб-сайты</p>
        </section>

        <section id="contact">
            <h2>Контакты</h2>
            <p>Email: example@mail.com</p>
        </section>
    </main>

    <footer>
        <p>© 2024 Мой Сайт</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.6;
}

header {
    background-color: #333;
    color: white;
    padding: 1rem;
}

nav ul {
    list-style: none;
    padding: 0;
    display: flex;
    gap: 2rem;
}

nav a {
    color: white;
    text-decoration: none;
}

main {
    padding: 2rem;
    max-width: 800px;
    margin: 0 auto;
}

section {
    margin: 2rem 0;
    padding: 2rem;
    border: 1px solid #ddd;
    border-radius: 8px;
}

button {
    padding: 0.5rem 1rem;
    background-color: #333;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 1rem;
    position: fixed;
    bottom: 0;
    width: 100%;
}

document.getElementById('changeColorBtn').addEventListener('click', function() {
    const colors = ['#ffcccc', '#ccffcc', '#ccccff', '#ffffcc'];
    const randomColor = colors[Math.floor(Math.random() * colors.length)];
    document.body.style.backgroundColor = randomColor;
});
