<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Impulse Dance Studio | Hip Hop Girly</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Raleway:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --black: #000000;
            --gold: #FFD700;
            --white: #FFFFFF;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Raleway', sans-serif;
            background-color: var(--black);
            color: var(--white);
            line-height: 1.6;
        }

        /* Шапка */
        .header {
            background: var(--black);
            padding: 1.5rem;
            position: fixed;
            width: 100%;
            z-index: 1000;
            border-bottom: 2px solid var(--gold);
        }

        .nav {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            color: var(--gold);
        }

        .nav-links {
            display: flex;
            gap: 2.5rem;
            list-style: none;
        }

        .nav-links a {
            color: var(--white);
            text-decoration: none;
            font-weight: 700;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--gold);
        }

        /* Герой-секция */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)),
                        url('https://images.unsplash.com/photo-1596386461350-326ccb383e9f') center/cover;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding-top: 80px;
        }

        .hero-content {
            max-width: 800px;
            padding: 0 20px;
        }

        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3.5rem;
            color: var(--gold);
            margin-bottom: 1.5rem;
        }

        /* Секция направлений */
        .directions {
            padding: 5rem 2rem;
            background: var(--white);
            color: var(--black);
        }

        .video-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .video-wrapper {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
        }

        .video-wrapper iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: 3px solid var(--gold);
        }

        /* Преподаватели */
        .instructors {
            padding: 5rem 2rem;
            background: var(--black);
        }

        .instructor-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            margin-top: 3rem;
        }

        .instructor-card {
            text-align: center;
            padding: 2rem;
            background: rgba(255,255,255,0.1);
            border-radius: 10px;
        }

        .instructor-img {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid var(--gold);
            margin-bottom: 1rem;
        }

        /* Форма записи */
        .booking {
            padding: 5rem 2rem;
            background: var(--white);
            color: var(--black);
            text-align: center;
        }

        .booking iframe {
            width: 100%;
            max-width: 800px;
            height: 800px;
            border: none;
            margin-top: 2rem;
        }

        /* Контакты */
        .contacts {
            padding: 5rem 2rem;
            text-align: center;
            background: var(--black);
        }

        .address {
            font-size: 1.5rem;
            margin: 2rem 0;
            color: var(--gold);
        }

        /* Адаптивность */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .instructor-img {
                width: 150px;
                height: 150px;
            }
        }
    </style>
</head>
<body>
    <header class="header">
        <nav class="nav">
            <div class="logo">IMPULSE</div>
            <ul class="nav-links">
                <li><a href="#home">Главная</a></li>
                <li><a href="#directions">Направления</a></li>
                <li><a href="#instructors">Преподаватели</a></li>
                <li><a href="#contacts">Контакты</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Hip Hop Girly в Филадельфии</h1>
            <p>Раскрой свою женственность через танец</p>
        </div>
    </section>

    <section class="directions" id="directions">
        <h2>Наши направления</h2>
        <div class="video-grid">
            <!-- Вставьте свои видео -->
            <div class="video-wrapper">
                <iframe src="https://www.youtube.com/embed/ВАШЕ_ВИДЕО" allowfullscreen></iframe>
            </div>
            <!-- Добавьте больше видео -->
        </div>
    </section>

    <section class="instructors" id="instructors">
        <h2>Наши преподаватели</h2>
        <div class="instructor-grid">
            <div class="instructor-card">
                <img src="https://example.com/instructor1.jpg" alt="Преподаватель" class="instructor-img">
                <h3>Анна Смит</h3>
                <p>Специалист по Hip Hop Girly</p>
            </div>
            <!-- Добавьте больше преподавателей -->
        </div>
    </section>

    <section class="booking" id="booking">
        <h2>Онлайн-запись</h2>
        <!-- Вставьте свою Google-форму -->
        <div class="google-form">
            [ВСТАВЬТЕ КОД ВАШЕЙ GOOGLE-ФОРМЫ]
        </div>
    </section>

    <section class="contacts" id="contacts">
        <h2>Контакты</h2>
        <div class="address">
            Philadelphia, 111 Buck Rd
        </div>
        <p>Телефон: (555) 123-4567</p>
        <p>Email: info@impulsedance.com</p>
    </section>
</body>
</html>