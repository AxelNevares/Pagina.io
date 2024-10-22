<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Actividad para probar GitHub</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f0f8ff;
            color: #333;
            text-align: center;
            margin: 0;
            padding: 50px;
        }
        h1 {
            font-size: 2.5em;
            margin-bottom: 20px;
            color: #2c3e50;
        }
        h2 {
            font-size: 2em;
            margin: 20px 0;
            color: #2980b9;
        }
        .container {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            padding: 30px;
            display: inline-block;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Actividad para probar GitHub</h1>
        <h2 id="hora"></h2>
    </div>

    <script>
        function mostrarHora() {
            const ahora = new Date();
            const opciones = { hour: '2-digit', minute: '2-digit', second: '2-digit' };
            document.getElementById('hora').innerText = ahora.toLocaleTimeString('es-ES', opciones);
        }
        
        mostrarHora();
        setInterval(mostrarHora, 1000);
    </script>
</body>
</html>