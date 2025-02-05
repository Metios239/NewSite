<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Feliz Aniversário!</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
            min-height: 100vh;
            background-color: #ffffff;
            position: relative;
            overflow-y: auto;
            text-align: center;
        }

        h1 {
            font-size: 2.5rem;
            color: #ff3366;
            text-shadow: 0 0 10px #ff6666, 0 0 20px #ff6699;
            animation: shine 2s infinite alternate, bounce 1s ease infinite;
            margin-top: 20px;
        }

        @keyframes shine {
            0% { text-shadow: 0 0 10px #ff6666, 0 0 20px #ff6699; }
            100% { text-shadow: 0 0 15px #ff6666, 0 0 25px #ff6699; }
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .heart {
            position: absolute;
            width: 30px;
            height: 30px;
            background-color: #ff6699;
            clip-path: polygon(50% 0%, 100% 35%, 80% 100%, 50% 75%, 20% 100%, 0% 35%);
            animation: heartbeat 1s infinite alternate, float 4s infinite ease-in-out;
        }

        @keyframes heartbeat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }

        @keyframes float {
            0% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0); }
        }

        .message {
            font-size: 1.5rem;
            color: #ff33cc;
            font-weight: bold;
            margin: 20px;
        }

        @media (max-width: 600px) {
            h1 {
                font-size: 2rem;
            }
            .message {
                font-size: 1.2rem;
            }
            .heart {
                width: 20px;
                height: 20px;
            }
        }
    </style>
</head>
<body>
    <h1>Feliz Aniversário, Alemoa Braba!</h1>

    <div class="message">Seu segundo presente será um Vale Resort. Partiu Praia do Rosa. Desejo tudo de bom, meu amor!</div>

    <!-- Corações -->
    <div class="heart" style="top: 100px; left: 10%;"></div>
    <div class="heart" style="top: 300px; left: 30%;"></div>
    <div class="heart" style="top: 500px; left: 70%;"></div>
    <div class="heart" style="top: 700px; left: 50%;"></div>

</body>
</html>
