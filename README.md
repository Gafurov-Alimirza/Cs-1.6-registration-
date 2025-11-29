# Cs-1.6-registration-
Чемпионат по кс 1.6  5х5 
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Регистрация – Чемпионат по CS 1.6</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: #0e0e0e;
            color: #f1f1f1;
            margin: 0;
            padding: 0;
        }
        header {
            background: #1a1a1a;
            padding: 20px;
            text-align: center;
            font-size: 26px;
            font-weight: bold;
            border-bottom: 2px solid #333;
        }
        .container {
            max-width: 600px;
            margin: 40px auto;
            background: #1c1c1c;
            padding: 30px;
            border-radius: 8px;
            border: 1px solid #333;
        }
        label {
            display: block;
            margin-top: 15px;
            font-size: 16px;
        }
        input {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            background: #2c2c2c;
            border: 1px solid #444;
            border-radius: 4px;
            color: #fff;
        }
        button {
            width: 100%;
            padding: 12px;
            background: #2f7bff;
            color: #fff;
            font-size: 18px;
            border: none;
            margin-top: 20px;
            cursor: pointer;
            border-radius: 4px;
        }
        button:hover { background: #1a5fff; }
    </style>
</head>
<body>

<header>Регистрация на Чемпионат по CS 1.6</header>

<div class="container">
    <form id="regForm">
        <label>ФИО</label>
        <input type="text" id="fio" required>

        <label>Ник в игре</label>
        <input type="text" id="nick" required>

        <label>Телефон</label>
        <input type="text" id="phone" required>

        <label>Название команды</label>
        <input type="text" id="team" required>

        <button type="submit">Отправить заявку</button>
    </form>
</div>

<script>
document.getElementById("regForm").addEventListener("submit", function(e) {
    e.preventDefault();

    const fio = document.getElementById("fio").value;
    const nick = document.getElementById("nick").value;
    const phone = document.getElementById("phone").value;
    const team = document.getElementById("team").value;

    const token =
