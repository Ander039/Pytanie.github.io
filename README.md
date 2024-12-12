
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pytanie</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #ffc0cb; /* Jasno różowy kolor tła */
            font-family: Arial, sans-serif;
        }
        .popup {
            background-color: white;
            border: 2px solid #ccc;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 20px;
            text-align: center;
            border-radius: 8px;
        }
        button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 4px;
            color: white;
            transition: transform 0.3s ease, background-color 0.3s ease;
        }
        button:hover {
            transform: scale(1.1); /* Powiększenie przy najechaniu */
        }
        button:active {
            transform: scale(0.9); /* Zmniejszenie przy kliknięciu */
        }
        .yes {
            background-color: #4caf50;
        }
        .yes:hover {
            background-color: #45a049; /* Jaśniejszy odcień zieleni */
        }
        .no {
            background-color: #f44336;
        }
        .no:hover {
            background-color: #e53935; /* Jaśniejszy odcień czerwieni */
        }
        .header {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <div class="header">Witajże moja lubo o mieniu Elżbieta</div>
    <div class="popup">
        <h1>Czy poślubisz mię?</h1>
        <button class="yes" onclick="sayYes()">A takoż</button>
        <button class="no" onclick="sayNo()">Nie raczę</button>
    </div>
    <script>
        function sayYes() {
            const popup = document.querySelector('.popup');
            popup.innerHTML = '<h1 style="color: green;">Raduję się, iż rzekłaś A takoż! ❤️</h1>';
        }
        function sayNo() {
            const popup = document.querySelector('.popup');
            popup.innerHTML = '<h1 style="color: red;">Wiem że to było przez przypadek...</h1>';
        }
    </script>
</body>
</html>
