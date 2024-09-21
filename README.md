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
            width: 90%;
            max-width: 800px;
            margin: 50px auto;
            padding: 40px;
            background-color: #ffffff; /* Weißer Hintergrund für den Inhalt */
            text-align: center;
            border: 10px solid #e0d8c3; /* Breiter Rahmen in hellem Goldton */
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            position: relative;
        }
        .container::before,
        .container::after {
            content: '';
            position: absolute;
            border: 1px solid #e0d8c3;
            width: calc(100% - 40px);
            height: calc(100% - 40px);
            top: 20px;
            left: 20px;
            pointer-events: none;
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
        <p>Wir laden euch herzlich ein, diesen besonderen Moment mit uns zu feiern!</p>
        <div class="date">06. September 2025</div>
        <!-- Button für Kalendereintrag -->
        <a href="data:text/calendar;charset=utf8,BEGIN:VCALENDAR%0AVERSION:2.0%0ABEGIN:VEVENT%0AUID:1234567890@example.com%0ADTSTAMP:20250906T080000Z%0AORGANIZER;CN=Calvin%20%26%20Iris:MAILTO:email@example.com%0ADTSTART:20250906T080000Z%0ADTEND:20250906T160000Z%0ASUMMARY:Calvin%20%26%20Iris%20Hochzeit%0ALOCATION:Berlin,%20Deutschland%0ADESCRIPTION:Einladung%20zur%20Hochzeit%20von%20Calvin%20%26%20Iris%20am%2006.%20September%202025.%0AEND:VEVENT%0AEND:VCALENDAR" class="calendar-button" download="calvin_iris_wedding.ics">Zum Kalender hinzufügen</a>
    </div>

    <footer>&copy; 2025 Calvin & Iris Hochzeit</footer>
</body>
</html>
