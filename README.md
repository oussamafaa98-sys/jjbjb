
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chronomètre</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
            background-color: #f0f0f0;
        }
        #chrono {
            font-size: 48px;
            margin-bottom: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Chronomètre</h1>
    <div id="chrono">00:00:00</div>
    <button id="startStop">Démarrer</button>
    <button id="reset">Réinitialiser</button>

    <script>
        let hours = 0;
        let minutes = 0;
        let seconds = 0;
        let interval;
        let running = false;

        const chrono = document.getElementById('chrono');
        const startStopBtn = document.getElementById('startStop');
        const resetBtn = document.getElementById('reset');

        function updateDisplay() {
            let h = hours.toString().padStart(2, '0');
            let m = minutes.toString().padStart(2, '0');
            let s = seconds.toString().padStart(2, '0');
            chrono.textContent = `${h}:${m}:${s}`;
        }

        function startStop() {
            if (!running) {
                interval = setInterval(() => {
                    seconds++;
                    if (seconds === 60) {
                        seconds = 0;
                        minutes++;
                    }
                    if (minutes === 60) {
                        minutes = 0;
                        hours++;
                    }
                    updateDisplay();
                }, 1000);
                startStopBtn.textContent = "Arrêter";
                running = true;
            } else {
                clearInterval(interval);
                startStopBtn.textContent = "Démarrer";
                running = false;
            }
        }

        function reset() {
            clearInterval(interval);
            hours = 0;
            minutes = 0;
            seconds = 0;
            updateDisplay();
            startStopBtn.textContent = "Démarrer";
            running = false;
        }

        startStopBtn.addEventListener('click', startStop);
        resetBtn.addEventListener('click', reset);
    </script>
</body>
</html>


