# impulsedancestudio
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dance Magic Studio</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: Arial, sans-serif; }
        
        /* Шапка */
        .header {
            background: #2c3e50;
            color: white;
            padding: 20px;
            text-align: center;
        }

        /* Основной контент */
        .hero {
            background: url('https://tinyurl.com/dance-bg') center/cover;
            height: 80vh;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }

        /* Кнопка */
        .cta-button {
            background: #e74c3c;
            color: white;
            padding: 15px 30px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }
        .cta-button:hover { background: #c0392b; }

        /* Адаптивность */
        @media (max-width: 768px) {
            .hero { height: 60vh; }
            h1 { font-size: 24px; }
        }
    </style>
</head>
<body>
    <header class="header">
        <h1>Dance Magic Studio</h1>
    </header>

    <div class="hero">
        <div>
            <h1>Научись танцевать за 1 месяц!</h1>
            <a href="#contact" class="cta-button">Записаться</a>
        </div>
    </div>
</body>
</html>