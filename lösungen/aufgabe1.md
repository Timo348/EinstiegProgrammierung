## index.html
``` 
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interaktive Begrüßung</title>
    <script src="javascript.js"></script>
</head>
<body>
    <h1>Willkommen</h1>
    <p>Bitte geben sie Ihren namen ein</p>
    <input type="text" id="InputName">
    <button type="button" onclick="NameFunktion()">Absenden</button>
    <p id="AusgabeName"></p>
</body>
</html>
``` 
## Javascript
``` 
function NameFunktion() {
    const name = document.getElementById("InputName").value;
    const ausgabe = document.getElementById("AusgabeName");

    ausgabe.textContent = "Hallo" + name;
}
``` 
