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
            background-color: #faf3e0; /* Sanfte, neutrale Hintergrundfarbe */
            color: #333;
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
            background-color: #faf3e0; /* Cremiger Hintergrund, der an Hochzeitseinladungen erinnert */
            padding: 20px;
            text-align: center;
            border: 2px solid #FFD700; /* Goldene Umrandung */
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2); /* Leichter Schatten für eleganten Effekt */
        }
        h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 4rem;
            color: #FFD700; /* Goldene Schrift für elegante Akzente */
            margin: 0;
        }
        h2 {
            font-size: 2.5rem;
            font-weight: bold;
            color: #333;
            margin: 20px 0;
        }
        p {
            font-size: 1.4rem;
            margin: 20px 0;
            color: #555;
        }
        .date {
            font-size: 2rem;
            font-weight: bold;
            color: #FFD700; /* Goldene Akzente */
            margin-bottom: 30px;
        }
        .calendar-button {
            text-decoration: none;
            background-color: #FFD700;
            color: #333;
            padding: 15px 30px;
            font-size: 1.2rem;
            border-radius: 30px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: background-color 0.3s ease, box-shadow 0.3s ease;
        }
        .calendar-button:hover {
            background-color: #f7c500;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
        }
        footer {
            position: absolute;
            bottom: 20px;
            font-size: 0.9rem;
            color: #888;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Save the Date!</h1>
        <h2>Calvin & Iris heiraten!</h2>
        <p>Wir laden euch herzlich ein, diesen besonderen Moment mit uns zu feiern!</p>
        <div class="date">Datum: 06. September 2025</div>
        <p>Eine formelle Einladung und weitere Informationen folgen bald.</p>
        <!-- Button für Kalendereintrag -->
        <a href="data:text/calendar;charset=utf8,BEGIN:VCALENDAR%0AVERSION:2.0%0ABEGIN:VEVENT%0AUID:1234567890@example.com%0ADTSTAMP:20250906T080000Z%0AORGANIZER;CN=Calvin%20%26%20Iris:MAILTO:email@example.com%0ADTSTART:20250906T080000Z%0ADTEND:20250906T160000Z%0ASUMMARY:Calvin%20%26%20Iris%20Hochzeit%0ALOCATION:Berlin,%20Deutschland%0ADESCRIPTION:Save%20the%20Date%20f%C3%BCr%20die%20Hochzeit%20von%20Calvin%20%26%20Iris%20am%2006.%20September%202025.%0AEND:VEVENT%0AEND:VCALENDAR" class="calendar-button" download="calvin_iris_wedding.ics">Zum Kalender hinzufügen</a>
    </div>

    <footer>&copy; 2025 Calvin & Iris Hochzeit</footer>
</body>
</html>
