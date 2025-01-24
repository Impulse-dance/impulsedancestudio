<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DanceLife Studio</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* Базовые стили */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            line-height: 1.6;
        }

        /* Шапка */
        header {
            background: #2c3e50;
            color: white;
            padding: 1rem;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        nav {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #e74c3c;
        }

        /* Герой-секция */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), 
                        url('https://images.unsplash.com/photo-1508700929628-666bc8bd84ea') center/cover;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            margin-top: 60px;
        }

        .hero-content h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
        }

        /* Секции */
        .section {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section h2 {
            text-align: center;
            margin-bottom: 3rem;
            color: #2c3e50;
        }

        /* Карточки направлений */
        .classes-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .class-card {
            background: #f9f9f9;
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s;
        }

        .class-card:hover {
            transform: translateY(-10px);
        }

        /* Форма записи */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }

        input, textarea {
            width: 100%;
            padding: 1rem;
            margin-bottom: 1rem;
            border: 2px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }

        button {
            background: #e74c3c;
            color: white;
            padding: 1rem 2rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.1rem;
            transition: background 0.3s;
        }

        button:hover {
            background: #c0392b;
        }

        /* Адаптивность */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero-content h1 {
                font-size: 2.5rem;
            }

            .section {
                padding: 3rem 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <h1>DanceLife</h1>
            <ul class="nav-links">
                <li><a href="#home">Главная</a></li>
                <li><a href="#classes">Направления</a></li>
                <li><a href="#contact">Контакты</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Преврати свое тело в инструмент</h1>
            <p>Профессиональное обучение современным танцам</p>
            <a href="#contact" class="btn">Записаться сейчас</a>
        </div>
    </section>

    <section class="section" id="classes">
        <h2>Наши направления</h2>
        <div class="classes-grid">
            <div class="class-card">
                <h3>Хип-Хоп</h3>
                <p>Базовые движения и связки</p>
                <p>🕒 Пн/Ср/Пт 19:00</p>
            </div>
            <div class="class-card">
                <h3>Contemporary</h3>
                <p>Современная пластика</p>
                <p>🕒 Вт/Чт 18:30</p>
            </div>
            <div class="class-card">
                <h3>Джаз-Фанк</h3>
                <p>Энергия и стиль</p>
                <p>🕒 Сб 12:00</p>
            </div>
        </div>
    </section>

    <section class="section" id="contact">
        <h2>Записаться на занятие</h2>
        <div class="contact-form">
            <form>
                <input type="text" placeholder="Ваше имя" required>
                <input type="email" placeholder="Ваш email" required>
                <select required>
                    <option value="">Выберите направление</option>
                    <option>Хип-Хоп</option>
                    <option>Contemporary</option>
                    <option>Джаз-Фанк</option>
                </select>
                <textarea placeholder="Комментарий" rows="4"></textarea>
                <button type="submit">Отправить заявку</button>
            </form>
        </div>
    </section>
</body>
</html>