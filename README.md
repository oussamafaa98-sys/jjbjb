<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Site de OUSSAMA POUR LE BANANE Banane 🍌</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fff9e6;
            color: #333;
        }

        header {
            background-color: #f2c94c;
            padding: 20px;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 2.5em;
        }

        nav {
            background-color: #f7d86a;
            padding: 10px;
            text-align: center;
        }

        nav a {
            margin: 0 15px;
            color: #333;
            text-decoration: none;
            font-weight: bold;
        }

        nav a:hover {
            text-decoration: underline;
        }

        main {
            padding: 20px;
            max-width: 900px;
            margin: auto;
        }

        .image-centre {
            text-align: center;
            margin-bottom: 20px;
        }

        .image-centre img {
            width: 300px;
            border-radius: 15px;
        }

        section {
            margin-bottom: 40px;
        }

        footer {
            background-color: #f2c94c;
            text-align: center;
            padding: 15px;
            position: relative;
            bottom: 0;
            width: 100%;
        }

        footer p {
            margin: 0;
        }
    </style>
</head>
<body>

    <header>
        <h1>Bienvenue sur le site de la Banane 🍌</h1>
        <p>Le fruit préféré des singes et des humains !</p>
    </header>

    <nav>
        <a href="#infos">Infos</a>
        <a href="#bienfaits">Bienfaits</a>
        <a href="#contact">Contact</a>
    </nav>

    <main>
        <div class="image-centre">
            <img src="https://upload.wikimedia.org/wikipedia/commons/8/8a/Banana-Single.jpg" alt="Banane">
        </div>

        <section id="infos">
            <h2>🍌 Informations sur la banane</h2>
            <p>La banane est un fruit tropical savoureux et riche en potassium. Elle pousse sur des bananiers et est consommée dans le monde entier.</p>
        </section>

        <section id="bienfaits">
            <h2>🌿 Bienfaits de la banane</h2>
            <ul>
                <li>Riche en énergie naturelle</li>
                <li>Source de vitamines et de potassium</li>
                <li>Améliore la digestion</li>
                <li>Bonne pour le moral 😄</li>
            </ul>
        </section>

        <section id="contact">
            <h2>📩 Contact</h2>
            <p>Envie d’en savoir plus sur la banane ?</p>
            <form>
                <label for="email">Votre email :</label><br>
                <input type="email" id="email" name="email" placeholder="exemple@email.com" required><br><br>
                <label for="message">Votre message :</label><br>
                <textarea id="message" name="message" rows="4" placeholder="Écrivez votre message ici..."></textarea><br><br>
                <button type="submit">Envoyer</button>
            </form>
        </section>
    </main>

    <footer>
        <p>© 2025 Site de Banane 🍌 — Fait avec amour et potassium</p>
    </footer>

</body>
</html>

    

