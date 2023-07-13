<html>
<head>
  <title>Bouton aléatoire</title>
  <style>
    #result {
      font-size: 24px;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <button onclick="afficherElementAleatoire()">Afficher une valeur aléatoire</button>
  <p id="result"></p>
  
  <script>
    var groupesMots = ["peinture", "cinéma", "mémoire", "site web", "broderie"];

    function afficherElementAleatoire() {
      var randomIndex = Math.floor(Math.random() * groupesMots.length);
      var resultElement = document.getElementById("result");
      resultElement.textContent = groupesMots[randomIndex];
    }
  </script>
</body>
</html>
