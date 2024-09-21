<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Save the Date: Calvin & Iris</title>
    <!-- Google Fonts für elegante Schrift -->
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Playfair Display', serif;
            background-color: #ADD8E6; /* Babyblauer Hintergrund */
            color: #00008B; /* Dunkelblaue Schrift */
            margin: 0;
            padding: 0;
        }
        .container {
            width: 100%;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background-color: #ADD8E6; /* Babyblauer Hintergrund */
            padding: 22px;  /* Vergrößert um 10% */
            text-align: center;
            border: 2.2px solid #00008B; /* Vergrößert um 10% */
            box-shadow: 0 8.8px 17.6px rgba(0, 0, 0, 0.2); /* Vergrößert um 10% */
        }
        h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 4.4rem; /* Vergrößert um 10% */
            color: #00008B;
            margin: 0;
        }
        h2 {
            font-size: 2.75rem; /* Vergrößert um 10% */
            font-weight: bold;
            color: #00008B;
            margin: 22px 0; /* Vergrößert um 10% */
        }
        p {
            font-size: 1.54rem; /* Vergrößert um 10% */
            margin: 22px 0; /* Vergrößert um 10% */
            color: #00008B;
        }
        .date {
            font-size: 2.2rem; /* Vergrößert um 10% */
            font-weight: bold;
            color: #00008B;
            margin-bottom: 33px; /* Vergrößert um 10% */
        }
        .calendar-button {
            text-decoration: none;
            background-color: #00008B;
            color: #ADD8E6;
            padding: 16.5px 33px; /* Vergrößert um 10% */
            font-size: 1.32rem; /* Vergrößert um 10% */
            border-radius: 33px; /* Vergrößert um 10% */
            box-shadow: 0 4.4px 8.8px rgba(0, 0, 0, 0.2); /* Vergrößert um 10% */
            transition: background-color 0.3s ease, box-shadow 0.3s ease;
        }
        .calendar-button:hover {
            background-color: #000070;
            box-shadow: 0 6.6px 13.2px rgba(0, 0, 0, 0.3); /* Vergrößert um 10% */
        }
        footer {
            position: absolute;
            bottom: 22px; /* Vergrößert um 10% */
            font-size: 0.99rem; /* Vergrößert um 10% */
            color: #00008B;
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
