<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Save the Date: Calvin & Iris</title>
    <!-- Google Fonts für elegante Schrift -->
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Playfair+Display:wght@400;700&family=Montserrat:wght@300;400&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #f8f4ef; /* Sanfter cremefarbener Hintergrund */
            color: #2f2f2f; /* Dunkles Grau für Schrift */
            margin: 0;
            padding: 0;
        }
        .container {
            width: 80%;
            max-width: 700px;
            height: auto;
            padding: 50px;
            margin: 50px auto;
            background-color: #ffffff; /* Weißer Hintergrund für den Inhalt */
            text-align: center;
            border: 10px solid transparent;
            position: relative;
            box-sizing: border-box;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }

        /* Erstelle floralen Rahmen mit Pseudo-Elementen */
        .container::before, .container::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            pointer-events: none;
            z-index: -1;
            border-radius: 20px;
        }

        .container::before {
            border: 2px solid #A0C77B; /* Grüner Rahmen ähnlich den Blättern */
            border-top-color: #D4AF37; /* Goldener Akzent */
            border-left-color: #D4AF37; /* Goldener Akzent */
        }

        .container::after {
            border: 2px solid transparent;
            box-shadow: 
                0 -10px 20px 5px rgba(212, 175, 55, 0.5), /* Oben goldene Schatten */
                10px 10px 20px 5px rgba(160, 199, 123, 0.5), /* Rechts grüne Schatten */
                -10px -10px 20px 5px rgba(160, 199, 123, 0.5), /* Links grüne Schatten */
                -10px 10px 20px 5px rgba(212, 175, 55, 0.5); /* Unten goldene Schatten */
        }

        h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 5rem;
            color: #c69c6d; /* Goldener Farbton */
            margin: 0;
        }

        h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            font-weight: 700;
            color: #2f2f2f;
            margin: 20px 0;
        }

        p {
            font-size: 1.2rem;
            margin: 20px 0;
            color: #4f4f4f;
        }

        .date {
            font-size: 2rem;
            font-weight: bold;
            color: #c69c6d; /* Goldener Farbton */
            margin-bottom: 30px;
        }

        .calendar-button {
            text-decoration: none;
            background-color: #c69c6d; /* Goldener Button */
            color: #ffffff;
            padding: 15px 30px;
            font-size: 1rem;
            border-radius: 5px;
            box-shadow: 0 5px 10px rgba(0, 0, 0, 0.1);
            transition: background-color 0.3s ease, box-shadow 0.3s ease;
        }

        .calendar-button:hover {
            background-color: #b2895b;
            box-shadow: 0 7px 14px rgba(0, 0, 0, 0.15);
        }

        footer {
            text-align: center;
            margin-top: 50px;
            font-size: 0.9rem;
            color: #7f7f7f;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Save the Date!</h1>
        <h2>Calvin & Iris heiraten!</h2>
        <p
