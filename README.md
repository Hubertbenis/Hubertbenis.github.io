<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hochzeit Registrierung</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            padding: 20px;
        }
        #additionalNames {
            display: none;
            margin-top: 10px;
        }
        #adminView {
            display: none;
            margin-top: 20px;
        }
        .highlight {
            font-weight: bold;
            color: red;
        }
    </style>
</head>
<body>
    <h1>Hochzeit Registrierung</h1>
    <p>Bitte geben Sie Ihren Namen ein:</p>
    <form id="nameForm">
        <label for="mainName">Name:</label>
        <input type="text" id="mainName" name="mainName" required>
        <button type="button" id="submitName">Bestätigen</button>
    </form>

    <div id="additionalNames">
        <p>Sie können zwei weitere Personen hinzufügen:</p>
        <form id="additionalForm">
            <label for="additionalName1">Zusatzperson 1:</label>
            <input type="text" id="additionalName1" name="additionalName1">
            <br>
            <label for="additionalName2">Zusatzperson 2:</label>
            <input type="text" id="additionalName2" name="additionalName2">
            <br>
            <button type="button" id="submitAdditional">Namen hinzufügen</button>
        </form>
    </div>

    <div id="adminView">
        <h2>Admin-Ansicht: Gesamtliste der Eingaben</h2>
        <ul id="adminList"></ul>
    </div>

    <script>
        // Datenbank-Simulation
        const database = [];

        document.getElementById('submitName').addEventListener('click', () => {
            const mainName = document.getElementById('mainName').value.trim();

            if (mainName === "") {
                alert("Bitte geben Sie einen Namen ein!");
                return;
            }

            if (mainName === "Admin123456") {
                showAdminView();
                return;
            }

            addNameToDatabase(mainName);
            document.getElementById('additionalNames').style.display = 'block';
        });

        document.getElementById('submitAdditional').addEventListener('click', () => {
            const additionalName1 = document.getElementById('additionalName1').value.trim();
            const additionalName2 = document.getElementById('additionalName2').value.trim();

            if (additionalName1) {
                addNameToDatabase(additionalName1, true);
            }

            if (additionalName2) {
                addNameToDatabase(additionalName2, true);
            }

            alert("Ihre Eingaben wurden gespeichert!");
            document.getElementById('additionalNames').style.display = 'none';
            document.getElementById('nameForm').reset();
            document.getElementById('additionalForm').reset();
        });

        function addNameToDatabase(name, isAdditional = false) {
            database.push({ name, isAdditional });
        }

        function showAdminView() {
            const adminList = document.getElementById('adminList');
            adminList.innerHTML = ""; // Reset list
            database.forEach(entry => {
                const listItem = document.createElement('li');
                listItem.textContent = entry.name;
                if (entry.isAdditional) {
                    listItem.classList.add('highlight');
                }
                adminList.appendChild(listItem);
            });

            document.getElementById('adminView').style.display = 'block';
        }
    </script>
</body>
</html>
