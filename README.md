<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Мир Scratch</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Roboto', sans-serif;
      line-height: 1.6;
      color: #333;
      background-color: #f5f5f5;
    }

    .header {
      background-color: #4CAF50;
      color: white;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 15px;
    }

    .logo-img {
      height: 50px;
    }

    .header h1 {
      margin: 0;
      font-size: 1.8rem;
    }

    .nav ul {
      list-style: none;
      display: flex;
      gap: 1.5rem;
    }

    .nav a {
      color: white;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s;
    }

    .nav a:hover {
      color: #ffeb3b;
    }

    .main {
      padding: 2rem;
    }

    .intro {
      text-align: center;
      margin-bottom: 2rem;
      padding: 1rem;
      background-color: white;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    }

    .intro h2 {
      margin-bottom: 1rem;
      color: #4CAF50;
    }

    .gallery {
      background-color: white;
      border-radius: 8px;
      padding: 1.5rem;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    }

    .gallery h2 {
      text-align: center;
      margin-bottom: 1.5rem;
      color: #4CAF50;
    }

    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
      padding: 1rem;
    }

    .gallery-item {
      text-align: center;
    }

    .gallery-item img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      transition: transform 0.3s;
    }

    .gallery-item img:hover {
      transform: scale(1.05);
    }

    .gallery-item p {
      margin-top: 0.5rem;
      font-weight: 500;
      color: #555;
    }

    .footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 1.5rem;
      margin-top: 2rem;
    }

    .footer p {
      margin: 0.5rem 0;
    }

    .footer a {
      color: #4CAF50;
      text-decoration: none;
      font-weight: 500;
    }

    .footer a:hover {
      text-decoration: underline;
    }

    @media (max-width: 768px) {
      .header {
        flex-direction: column;
        text-align: center;
      }

      .nav ul {
        margin-top: 1rem;
        flex-wrap: wrap;
        justify-content: center;
      }

      .main {
        padding: 1rem;
      }
    }
  </style>
</head>
<body>
  <header class="header">
    <div class="logo">
      <img src="scratch-logo.png" alt="Логотип Scratch" class="logo-img">
      <h1>Мир Scratch</h1>
    </div>
    <nav class="nav">
      <ul>
        <li><a href="#gallery">Галерея</a></li>
        <li><a href="https://scratch.mit.edu" target="_blank">Официальный сайт</a></li>
        <li><a href="https://scratch.mit.edu/projects/editor" target="_blank">Создать проект</a></li>
      </ul>
    </nav>
  </header>

  <main class="main">
    <section class="intro">
      <h2>Что такое Scratch?</h2>
      <p>Scratch — это визуальный язык программирования для детей и начинающих. С его помощью можно создавать анимации, игры и интерактивные истории, соединяя цветные блоки-команды.</p>
    </section>

    <section id="gallery" class="gallery">
      <h2>Галерея проектов</h2>
      <div class="gallery-grid">
        <div class="gallery-item">
          <img src="project1.jpg" alt="Проект 1">
          <p>Игра «Лабиринт»</p>
        </div>
        <div class="gallery-item">
          <img src="project2.jpg" alt="Проект 2">
          <p>Анимация «Кот и мяч»</p>
        </div>
        <div class="gallery-item">
          <img src="project3.jpg" alt="Проект 3">
          <p>История «Путешествие в космос»</p>
        </div>
        <div class="gallery-item">
          <img src="project4.jpg" alt="Проект 4">
          <p>Симулятор «Ферма»</p>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <p>&copy; 2025 Мир Scratch. Все права защищены.</p>
    <p>
      <a href="https://scratch.mit.edu" target="_blank">Scratch MIT</a> | 
      <a href="https://edu.scratch.mit.edu" target="_blank">Обучение Scratch</a>
    </p>
  </footer>
</body>
</html>
