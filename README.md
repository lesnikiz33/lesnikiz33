<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Мой первый Mini App</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
            background-color: #f0f4f8;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <h1>Привет из Mini App!</h1>
    <p>Здесь будет CRM для тенниса</p>
    <button onclick="showAlert()">Нажми меня</button>

    <script>
        function showAlert() {
            Telegram.WebApp.showAlert('Привет, ' + Telegram.WebApp.initDataUnsafe.user?.first_name || 'Пользователь!');
        }
    </script>
</body>
</html>
