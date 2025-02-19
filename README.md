<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Твой персональный тренер</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background: url('https://source.unsplash.com/featured/?fitness') no-repeat center center/cover;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh; /* Ensure full viewport height */
            color: white;
            text-align: center;
        }

        .container {
            background: rgba(0, 0, 0, 0.7);
            padding: 40px; /* Increased padding */
            border-radius: 15px; /* More rounded corners */
            max-width: 700px; /* Increased max-width */
            width: 90%; /* Responsive width */
            box-shadow: 0 0 20px rgba(255, 255, 255, 0.2); /* Added shadow */
        }

        h1 {
            font-size: 2.5em; /* Increased font size */
            margin-bottom: 20px;
        }

        h2 {
            font-size: 1.8em; /* Increased font size */
            margin-top: 30px;
        }

        p {
            font-size: 1.2em; /* Increased font size */
            line-height: 1.6; /* Improved readability */
            margin-bottom: 15px;
        }

        .stats {
            font-weight: bold;
            font-size: 1.3em; /* Increased font size */
        }

        .button {
            display: inline-block;
            padding: 15px 30px; /* Increased padding */
            background-color: #007bff;
            color: white;
            text-decoration: none;
            border-radius: 8px; /* More rounded corners */
            font-size: 1.2em; /* Increased font size */
            margin-top: 20px;
            transition: background-color 0.3s ease; /* Smooth transition */
        }

        .button:hover {
            background-color: #0056b3; /* Darker color on hover */
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Привет! Я твой онлайн-тренер</h1>
        <p>Меня зовут <strong>ДАНИЛО</strong>, и я помогу тебе достичь твоих фитнес-целей!</p>

        <h2>Мои достижения:</h2>
        <p> Победитель чемпионата Украины</p>
        <p> Опыт работы с атлетами разного уровня</p>

        <h2>Силовые показатели:</h2>
        <p class="stats">Жим лёжа: 140 кг</p>
        <p class="stats">Приседание: 220 кг</p>
        <p class="stats">Становая тяга: 250 кг</p>

        <p><strong>Готов начать свой путь к лучшей форме?</strong></p>
        <a href="#" class="button">Записаться на тренировку</a>
    </div>
</body>
</html>
