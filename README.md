<!DOCTYPE html>
<html lang="fr" dir="ltr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Maths Pro - Exercices & Cours</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #2563eb; /* Bleu moderne */
            --secondary-color: #10b981; /* Vert réussite */
            --accent-color: #f59e0b; /* Orange attention */
            --dark-bg: #1e293b;
            --light-bg: #f8fafc;
            --text-color: #334155;
            --card-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--light-bg);
            color: var(--text-color);
            line-height: 1.6;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, var(--primary-color), #1e40af);
            color: white;
            padding: 3rem 1rem;
            text-align: center;
            border-radius: 0 0 50px 50px;
            margin-bottom: 3rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        header h1 {
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
            letter-spacing: 1px;
        }

        header p {
            font-size: 1.1rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
        }

        /* Main Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1.5rem;
        }

        /* Section Titles */
        .section-title {
            text-align: center;
            font-size: 2rem;
            color: var(--dark-bg);
            margin-bottom: 2rem;
            position: relative;
            display: inline-block;
            width: 100%;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background-color: var(--accent-color);
            margin: 10px auto 0;
            border-radius: 2px;
        }

        /* Cards Grid */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }

        /* Level Card */
        .level-card {
            background: white;
            border-radius: 16px;
            padding: 2rem;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: var(--card-shadow);
            border-top: 5px solid transparent;
            position: relative;
            overflow: hidden;
        }

        .level-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.15);
        }

        /* Specific Colors for Levels */
        .college-card { border-color: var(--secondary-color); }
        .lycee-card { border-color: var(--primary-color); }

        .level-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
            display: inline-block;
        }

        .level-title {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: var(--dark-bg);
        }

        .level-desc {
            font-size: 0.95rem;
            color: #64748b;
            margin-bottom: 1.5rem;
        }

        /* Buttons */
        .btn {
            display: inline-block;
            padding: 0.8rem 1.5rem;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.3s ease;
            width: 100%;
        }

        .btn-college {
            background-color: rgba(16, 185, 129, 0.1);
            color: var(--secondary-color);
        }
        .btn-college:hover {
            background-color: var(--secondary-color);
            color: white;
        }

        .btn-lycee {
            background-color: rgba(37, 99, 235, 0.1);
            color: var(--primary-color);
        }
        .btn-lycee:hover {
            background-color: var(--primary-color);
            color: white;
        }

        /* Footer */
        footer {
            background-color: var(--dark-bg);
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
        }

        footer p {
            opacity: 0.7;
            font-size: 0.9rem;
        }

        /* Responsive Adjustments */
        @media (max-width: 768px) {
            header h1 { font-size: 2rem; }
            .section-title { font-size: 1.75rem; }
        }
    </style>
</head>
<body>

    <!-- En-tête -->
    <header>
        <div class="container">
            <h1>Maths Pro</h1>
            <p>Votre plateforme d'excellence pour maîtriser les mathématiques du collège au lycée.</p>
        </div>
    </header>

    <div class="container">

        <!-- Section Collège -->
        <section id="college">
            <h2 class="section-title">Niveau Collège</h2>
            <div class="grid">
                <!-- 1ère Année -->
                <div class="level-card college-card">
                    <span class="level-icon">1️⃣</span>
                    <h3 class="level-title">1ère Année (1AC)</h3>
                    <p class="level-desc">Bases de l'algèbre, géométrie et calcul numérique.</p>
                    <a href="college/1ac.html" class="btn btn-college">Voir les Exercices</a>
                </div>

                <!-- 2ème Année -->
                <div class="level-card college-card">
                    <span class="level-icon">2️⃣</span>
                    <h3 class="level-title">2ème Année (2AC)</h3>
                    <p class="level-desc">Approfondissement, équations et symétrie.</p>
                    <a href="college/2ac.html" class="btn btn-college">Voir les Exercices</a>
                </div>

                <!-- 3ème Année -->
                <div class="level-card college-card">
                    <span class="level-icon">3️⃣</span>
                    <h3 class="level-title">3ème Année (3AC)</h3>
                    <p class="level-desc">Préparation au brevet, fonctions et théorèmes clés.</p>
                    <a href="college/3ac.html" class="btn btn-college">Voir les Exercices</a>
                </div>
            </div>
        </section>

        <!-- Section Lycée -->
        <section id="lycee">
            <h2 class="section-title">Niveau Lycée</h2>
            <div class="grid">
                <!-- Tronc Commun -->
                <div class="level-card lycee-card">
                    <span class="level-icon">⚛️</span>
                    <h3 class="level-title">Tronc Commun</h3>
                    <p class="level-desc">Socle scientifique, vecteurs et ensembles de nombres.</p>
                    <a href="lycee/tc.html" class="btn btn-lycee">Voir les Exercices</a>
                </div>

                <!-- 1ère Bac -->
                <div class="level-card lycee-card">
                    <span class="level-icon">📈</span>
                    <h3 class="level-title">1ère Année Bac</h3>
                    <p class="level-desc">Étude de fonctions, suites et barycentre.</p>
                    <a href="lycee/1bac.html" class="btn btn-lycee">Voir les Exercices</a>
                </div>

                <!-- 2ème Bac -->
                <div class="level-card lycee-card">
                    <span class="level-icon">🎓</span>
                    <h3 class="level-title">2ème Année Bac</h3>
                    <p class="level-desc">Préparation au baccalauréat : Analyse, Complexes, Probas.</p>
                    <a href="lycee/2bac.html" class="btn btn-lycee">Voir les Exercices</a>
                </div>
            </div>
        </section>

    </div>

    <!-- Pied de page -->
    <footer>
        <div class="container">
            <p>&copy; 2025 Maths Pro. Tous droits réservés.</p>
            <p>Conçu pour la réussite scolaire.</p>
        </div>
    </footer>

</body>
</html>
