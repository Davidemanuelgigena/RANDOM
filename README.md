<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Novia 2025</title>
  <style>
    body {
      font-family: sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 50px;
      background: #f0f0f0;
    }
    .switch-group {
      margin: 10px 0;
    }
    label {
      font-size: 1.2em;
      margin-left: 10px;
    }
  </style>
</head>
<body>

  <h2>Encontrar una novia en 2025:</h2>

  <div class="switch-group">
    <input type="checkbox" id="libre">
    <label for="libre">Libre de bendiciones</label>
  </div>

  <div class="switch-group">
    <input type="checkbox" id="hermosa">
    <label for="hermosa">Hermosa</label>
  </div>

  <div class="switch-group">
    <input type="checkbox" id="estable">
    <label for="estable">Mentalmente estable</label>
  </div>

  <script>
    const libre = document.getElementById("libre");
    const hermosa = document.getElementById("hermosa");
    const estable = document.getElementById("estable");

    function controlarChecks() {
      const activados = [libre, hermosa, estable].filter(c => c.checked);
      if (activados.length > 2) {
        this.checked = false;
      }
    }

    libre.addEventListener("change", controlarChecks);
    hermosa.addEventListener("change", controlarChecks);
    estable.addEventListener("change", controlarChecks);
  </script>

</body>
</html>
