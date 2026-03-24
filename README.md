<!DOCTYPE html>
<html>
<head>
  <title>Tienda Ridouane</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body { font-family: Arial; margin: 0; background: #f2f2f2; }
    header { background: #2c3e50; color: white; padding: 15px; text-align: center; }
    h2 { margin-left: 10px; }
    .contenedor { display: flex; flex-wrap: wrap; justify-content: center; }
    .producto {
      background: white;
      width: 90%;
      max-width: 300px;
      margin: 10px;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    }
    img { width: 100%; }
    .info { padding: 10px; }
    button {
      background: #25D366;
      color: white;
      border: none;
      padding: 10px;
      width: 100%;
      border-radius: 5px;
      font-size: 16px;
    }
  </style>
</head>

<body>

<header>
  <h1>Tienda Ridouane</h1>
  <p>Alimentación y decoración</p>
</header>

<h2>Alimentación</h2>
<div class="contenedor">

  <div class="producto">
    <img src="https://via.placeholder.com/300">
    <div class="info">
      <h3>Lentejas</h3>
      <p>1kg - 2€</p>
      <button onclick="comprar('Lentejas 1kg')">Comprar</button>
    </div>
  </div>

  <div class="producto">
    <img src="https://via.placeholder.com/300">
    <div class="info">
      <h3>Galletas</h3>
      <p>Paquete - 1.50€</p>
      <button onclick="comprar('Galletas')">Comprar</button>
    </div>
  </div>

</div>

<h2>Decoración</h2>
<div class="contenedor">

  <div class="producto">
    <img src="https://via.placeholder.com/300">
    <div class="info">
      <h3>Flores artificiales</h3>
      <p>Ramo - 5€</p>
      <button onclick="comprar('Flores artificiales')">Comprar</button>
    </div>
  </div>

</div>

<script>
function comprar(producto) {
  let telefono = "34600000000"; // CAMBIA por tu número
  let mensaje = "Hola, quiero comprar: " + producto;
  window.open("https://wa.me/" + telefono + "?text=" + encodeURIComponent(mensaje));
}
</script>

</body>
</html>
