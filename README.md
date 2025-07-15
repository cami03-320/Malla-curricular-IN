# Malla-curricular-IN
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Malla Curricular Interactiva</title>
  <style>
    body { font-family: Arial; margin: 20px; background: #f4f4f4; }
    .curso { background: white; padding: 15px; border-radius: 10px; margin-bottom: 10px; box-shadow: 0 0 5px #ccc; }
    .detalle { display: none; margin-top: 10px; }
    button { background: #007bff; color: white; border: none; padding: 5px 10px; border-radius: 5px; cursor: pointer; }
  </style>
</head>
<body>
  <h1>Malla Curricular - Enfermería</h1>

  <div class="curso">
    <strong>Anatomía Humana</strong> - 1° Ciclo
    <br><button onclick="toggleDetalle(this)">Ver más</button>
    <div class="detalle">
      <p>Créditos: 4</p>
      <p>Descripción: Estudio de la estructura del cuerpo humano.</p>
      <p>Prerrequisito: Ninguno</p>
    </div>
  </div>

  <div class="curso">
    <strong>Fundamentos de Enfermería</strong> - 1° Ciclo
    <br><button onclick="toggleDetalle(this)">Ver más</button>
    <div class="detalle">
      <p>Créditos: 3</p>
      <p>Descripción: Introducción a la práctica de enfermería profesional.</p>
      <p>Prerrequisito: Ninguno</p>
    </div>
  </div>

  <script>
    function toggleDetalle(btn) {
      const detalle = btn.nextElementSibling;
      detalle.style.display = (detalle.style.display === 'block') ? 'none' : 'block';
      btn.textContent = (detalle.style.display === 'block') ? 'Ocultar' : 'Ver más';
    }
  </script>
</body>
</html>
