<details>
<summary>💻 Voir le code complet GAZO WORLD</summary>

```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>GAZO WORLD</title>
  <link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      background-color: black;
      color: #00ff00;
      font-family: 'Share Tech Mono', monospace;
      overflow: hidden;
}

.matrix {
      position: fixed;
      top: 0; left: 0;
      width: 100vw;
      height: 100vh;
      background-image: url('https://raw.githubusercontent.com/ManzDev/cursos-assets/main/animated-stars.gif');
      opacity: 0.15;
      pointer-events: none;
      z-index: -1;
}

.container {
      padding: 80px 20px;
      text-align: center;
}

    h1 {
      font-size: 3em;
      animation: blink 1s infinite;
      cursor: pointer;
}

    @keyframes blink {
      50% {opacity: 0.6;}
}

.terminal {
      margin-top: 40px;
      text-align: left;
      max-width: 600px;
      margin-left: auto;
      margin-right: auto;
      padding: 20px;
      border: 2px solid #00ff00;
      background: rgba(0, 0, 0, 0.8);
}

.terminal input {
      background: transparent;
      border: none;
      border-bottom: 1px solid #00ff00;
      color: #00ff00;
      font-family: inherit;
      font-size: 1em;
      width: 100%;
      margin-top: 10px;
}

    button {
      margin-top: 20px;
      background: #00ff00;
      color: black;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      font-family: inherit;
      font-weight: bold;
}

    button:hover {
      background: lime;
}
  </style>
</head>
<body>
  <div class="matrix"></div>
  <div class="container">
    <h1 onclick="document.getElementById('sound').play()">GAZO WORLD</h1>

    <div class="terminal">
      <p>> Authentification requise:</p>
      <input type="text" placeholder="Nom d'utilisateur">
      <input type="password" placeholder="Mot de passe">
      <button onclick="auth()">Connexion</button>
    </div>

    <audio id="sound" src="https://www.soundjay.com/button/beep-07.mp3" preload="auto"></audio>
  </div>

  <script>
    function auth() {
      alert("⛔ Accès refusé. Système sécurisé GAZO.");
}
  </script>
</body>
</html>
