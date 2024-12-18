# page
site
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Spécialiste du nettoyage après décès, nettoyage syndrome de Diogène et nettoyage extrême dans les Alpes-Maritimes et le Var. Service rapide, efficace et discret.">
    <meta name="keywords" content="nettoyage après décès, nettoyage syndrome de Diogène, nettoyage extrême, débarras, Alpes-Maritimes, Var, Cannes">
    <meta name="author" content="Votre Nom ou Entreprise">
    <title>Nettoyage Après Décès & Syndrome de Diogène - Alpes-Maritimes & Var</title>
    <link href="https://fonts.googleapis.com/css2?family=Cardo:wght@400;700&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background: linear-gradient(45deg, #001529, #00334d); /* Fond animé bleu nuit */
            animation: backgroundMove 10s ease infinite;
            color: #ffffff;
            margin: 0;
            padding: 0;
            overflow-x: hidden; /* Empêche le défilement horizontal */
        }

        /* Animation du fond avec un mouvement fluide */
        @keyframes backgroundMove {
            0% {
                background-position: 0 0;
            }
            100% {
                background-position: 200% 200%;
            }
        }

        header {
            background-color: rgba(51, 51, 51, 0.9); /* Légèrement transparent */
            padding: 30px 0;
            text-align: center;
            border-bottom: 2px solid #ccc;
            position: relative;
            overflow: hidden;
        }

        header h1 {
            font-family: 'Cardo', serif;
            color: #f4f4f4;
            font-size: 2.5em;
            margin: 0;
            text-transform: uppercase;
            letter-spacing: 2px;
            position: relative;
        }

        /* Effet de reflet sous le titre */
        header h1::after {
            content: "";
            position: absolute;
            bottom: -20px;
            left: 0;
            width: 100%;
            height: 20px;
            background: rgba(255, 255, 255, 0.2);
            transform: scaleY(-1);
            filter: blur(2px);
            opacity: 0.5;
        }

        main {
            padding: 20px;
        }

        section {
            margin-bottom: 30px;
            opacity: 0;
            transform: translateY(50px);
            transition: transform 0.5s ease-out, opacity 0.5s ease-out;
        }

        section.visible {
            opacity: 1;
            transform: translateY(0);
        }

        section h2 {
            color: #f4f4f4;
            text-align: center;
            font-size: 1.8em;
            margin-bottom: 10px;
        }

        section p, section ul {
            text-align: center;
            font-size: 1.1em;
        }

        section ul {
            list-style: none;
            padding: 0;
        }

        section ul li {
            margin: 10px 0;
        }

        footer {
            background-color: rgba(51, 51, 51, 0.9);
            color: #f4f4f4;
            text-align: center;
            padding: 20px;
            border-top: 2px solid #ccc;
        }

        .cta {
            display: inline-block;
            background-color: #005f7a;
            padding: 15px 30px;
            border-radius: 5px;
            font-size: 1.2em;
            color: #fff;
            text-decoration: none;
            text-align: center;
            margin-top: 20px;
            transition: background-color 0.3s ease;
        }

        .cta:hover {
            background-color: #004c61;
        }

        .keywords {
            text-align: center;
            margin: 20px 0;
            font-size: 1.2em;
            font-weight: bold;
            color: #f4f4f4;
        }

        .phone-number {
            font-size: 2em; /* Numéro de téléphone agrandi */
            font-weight: bold;
            color: #f4f4f4;
        }

        @media (max-width: 768px) {
            body {
                font-size: 1em;
            }
            header h1 {
                font-size: 2em;
            }
            .cta {
                font-size: 1em;
                padding: 10px 20px;
            }
            .phone-number {
                font-size: 1.5em; /* Réduire la taille sur les petits écrans */
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Nettoyage Décès</h1>
    </header>
    <main>
        <section id="services">
            <h2>Nos Services</h2>
            <ul>
                <li>Nettoyage après décès</li>
                <li>Débarras et nettoyage pour syndrome de Diogène</li>
                <li>Nettoyage extrême pour situations difficiles</li>
            </ul>
        </section>
        <section id="pourquoi">
            <h2>Pourquoi Nous Choisir ?</h2>
            <p>Avec une approche méthodique et professionnelle, nous garantissons :</p>
            <ul>
                <li>&#8226; Écoute</li>
                <li>&#8226; Discrétion</li>
                <li>&#8226; Confiance</li>
            </ul>
        </section>
        <section id="zones">
            <h2>Zones d'Intervention</h2>
            <p>Nous intervenons rapidement dans les <strong>Alpes-Maritimes</strong> et le <strong>Var</strong>.</p>
        </section>
        <section id="contact">
            <h2>Contactez-Nous</h2>
            <p>Appelez-nous au <span class="phone-number">06 86 06 62 60</span> ou envoyez un email à <strong>contact.nettoyagedeces@gmail.com</strong>.</p>
            <a class="cta" href="tel:0686066260">Appelez Maintenant</a>
        </section>
        <div class="keywords">
            Nettoyage Après Décès | Nettoyage Syndrome de Diogène | Nettoyage Extrême
        </div>
    </main>
    <footer>
        <p>&copy; 2024 Nettoyage Décès. Tous droits réservés.</p>
    </footer>

    <script>
        // Animation des sections lors du défilement
        const sections = document.querySelectorAll('section');

        function checkVisibility() {
            const triggerBottom = window.innerHeight / 1.2;
            sections.forEach(section => {
                const sectionTop = section.getBoundingClientRect().top;
                if (sectionTop < triggerBottom) {
                    section.classList.add('visible');
                }
            });
        }

        window.addEventListener('scroll', checkVisibility);
        checkVisibility(); // On vérifie la visibilité dès le chargement de la page
    </script>
</body>
</html>
