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
            background: url('https://source.unsplash.com/featured/?gym,fitness') no-repeat center center/cover;
            min-height: 100vh;
            color: white;
            display: flex;
            flex-direction: column;
        }

        .container {
            background: rgba(0, 0, 0, 0.7);
            padding: 40px;
            border-radius: 15px;
            max-width: 700px;
            width: 90%;
            box-shadow: 0 0 20px rgba(255, 255, 255, 0.2);
            margin: auto; /* Центрируем контейнер по горизонтали */
            margin-top: 50px; /* Добавляем отступ сверху */
        }

        h1 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }

        h2 {
            font-size: 1.8em;
            margin-top: 30px;
        }

        p {
            font-size: 1.2em;
            line-height: 1.6;
            margin-bottom: 15px;
        }

        .stats {
            font-weight: bold;
            font-size: 1.3em;
        }

        .button {
            display: inline-block;
            padding: 15px 30px;
            background-color: #007bff;
            color: white;
            text-decoration: none;
            border-radius: 8px;
            font-size: 1.2em;
            margin-top: 20px;
            transition: background-color 0.3s ease;
        }

        .button:hover {
            background-color: #0056b3;
        }

        #modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.4);
        }

        .modal-content {
            background-color: #fefefe;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
        }

        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }

        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
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
        <a href="#" class="button" id="openModal">Записаться на тренировку</a>
    </div>

    <div id="modal">
        <div class="modal-content">
            <span class="close" id="closeModal">&times;</span>
            <h2>Запись на тренировку</h2>
            <p><strong>Инструкция:</strong></p>
            <p>Свяжитесь со мной в Instagram или Telegram, чтобы выбрать удобное время и обсудить детали тренировок:</p>
            <p><strong>Instagram:</strong> <a href="https://www.instagram.com/xxeggrts" target="_blank">@xxeggrts</a></p>
            <p><strong>Telegram:</strong> <a href="https://t.me/Xxeggrts" target="_blank">@Xxeggrts</a></p>
        </div>
    </div>

    <script>
        const modal = document.getElementById("modal");
        const openModalBtn = document.getElementById("openModal");
        const closeModalBtn = document.getElementById("closeModal");

        openModalBtn.onclick = function () {
            modal.style.display = "block";
        }

        closeModalBtn.onclick = function () {
            modal.style.display = "none";
        }

        window.onclick = function (event) {
            if (event.target == modal) {
                modal.style.display = "none";
            }
        }
    </script>
</body>

</html>
