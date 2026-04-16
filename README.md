<!DOCTYPE html>
<html lang="cs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Továrna na kontakty | E-mailový Magnet</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --pozadi: #0a2c21; /* Tmavá profi zelená ze vzoru */
            --zlata: #d4af37;
            --text: #ffffff;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Montserrat', sans-serif;
            background-color: var(--pozadi);
            color: var(--text);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        .wrapper {
            max-width: 1100px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            padding: 40px;
            align-items: center;
        }

        /* Mobilní verze - pod sebou */
        @media (max-width: 768px) {
            .wrapper { grid-template-columns: 1fr; text-align: center; }
            .book-img { order: -1; padding: 0 40px; } /* Kniha nahoře s větším paddingem */
        }

        h1 {
            font-size: 3rem;
            font-weight: 800;
            line-height: 1.1;
            margin-bottom: 20px;
        }

        span.highlight { color: var(--zlata); }

        p {
            font-size: 1.2rem;
            line-height: 1.6;
            margin-bottom: 35px;
            opacity: 0.9;
        }

        .btn {
            background-color: var(--zlata);
            color: #000;
            padding: 20px 40px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1rem;
            border-radius: 5px;
            text-transform: uppercase;
            transition: all 0.3s ease;
            display: inline-block;
            box-shadow: 0 10px 20px rgba(0,0,0,0.3);
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 25px rgba(0,0,0,0.4);
            filter: brightness(1.1);
        }

        /* Styl pro zobrazení knihy */
        .book-img {
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .book-img img {
            width: 100%;
            max-width: 400px;
            height: auto;
            /* Triky pro oříznutí šedého pozadí */
            object-fit: cover;
            border-radius: 5px;
            /* Stín, který splyne s novým zeleným pozadím */
            filter: drop-shadow(0px 10px 30px rgba(0,0,0,0.5));
            /* Jemné zvětšení ořezu, aby zmizely hrany šedého mockupu */
            transform: scale(1.02);
        }
    </style>
</head>
<body>

    <div class="wrapper">
        <div class="content">
            <h1>Spusťte svou <span class="highlight">Továrnu na kontakty</span> a prodávejte víc</h1>
            <p>Získejte praktický e-book, který vás naučí, jak proměnit návštěvníky webu v loajální zákazníky. Kompletní návod na sběr a správu kontaktů.</p>
            <a href="#" class="btn">Chci e-book hned teď zdarma</a>
        </div>
        <div class="book-img">
            <img src="kniha.png" alt="Továrna na kontakty - E-book">
        </div>
    </div>

</body>
</html>
