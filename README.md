!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Una pregunta importante...</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      text-align: center;
      margin-top: 100px;
      background-color: #570526;
    } 
    h1 {
      color: #d4950b;
    }
    button {
      padding: 15px 30px;
      font-size: 18px;
      margin: 10px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: all 0.3s ease;
    }
    #yes {
      background-color: #28a745;
      color: white;
    }
    #no {
      background-color: #dc3545;
      color: white;
      position: absolute;
    }
  </style>
</head>
<body>
  <h1>¿Quieres ser mi novia?</h1>
  <button id="yes" onclick="respuestaSi()">Sí</button>
  <button id="no" onmouseover="moverBoton()">No</button>

  <script>
    function respuestaSi() {
      alert("¡Sabía que dirías que sí! Te quiero mucho.");
    }

    function moverBoton() {
      const noBtn = document.getElementById('no');
      const x = Math.floor(Math.random() * window.innerWidth - 100);
      const y = Math.floor(Math.random() * window.innerHeight - 100);
      noBtn.style.left = `${x}px`;
      noBtn.style.top = `${y}px`;
    }
  </script>
</body>
</html>
