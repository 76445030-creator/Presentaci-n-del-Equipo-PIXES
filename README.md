<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Infografía Extendida: Regresión Logística para Clasificación de Imágenes (Gato vs. Perro)</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f4f7f9;
            color: #333;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }

        .infographic-container {
            max-width: 1100px;
            margin: 40px auto;
            background-color: #ffffff;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            border-radius: 12px;
            overflow: hidden;
        }

        header {
            background: linear-gradient(90deg, #1a73e8, #0049b7);
            color: white;
            padding: 30px;
            text-align: center;
            border-top-left-radius: 12px;
            border-top-right-radius: 12px;
        }

        header h1 {
            margin: 0 0 10px 0;
            font-size: 2.4em;
            font-weight: 700;
        }

        header p {
            margin: 5px 0 0 0;
            font-size: 1.1em;
            font-weight: 300;
        }

        .integrantes {
            background-color: #0c62e1;
            padding: 10px;
            font-size: 1em;
            font-weight: 600;
        }

        .integrantes span {
            display: block;
            margin-top: 5px;
        }

        .content-section {
            padding: 30px;
        }

        h2 {
            color: #1a73e8;
            border-bottom: 3px solid #e0e0e0;
            padding-bottom: 10px;
            margin-top: 30px;
            font-weight: 600;
            font-size: 1.8em;
        }

        .highlight {
            background-color: #e8f0fe;
            border-left: 5px solid #1a73e8;
            padding: 15px;
            margin: 20px 0;
            border-radius: 8px;
            font-weight: 500;
        }

        .formula {
            background: #000;
            color: #0f0;
            font-family: monospace;
            padding: 15px;
            border-radius: 8px;
            font-size: 1.2em;
            text-align: center;
        }

        .process-steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .step {
            background: #fff3e0;
            border: 1px solid #ffb74d;
            border-radius: 8px;
            padding: 20px;
            text-align: center;
        }

        .step h4 {
            color: #e65100;
            margin-top: 0;
        }

        .pros-cons {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
        }

        .pros, .cons {
            flex: 1;
            padding: 20px;
            border-radius: 8px;
        }

        .pros {
            background-color: #e6f4ea;
            border: 2px solid #34a853;
        }

        .cons {
            background-color: #fce8e6;
            border: 2px solid #ea4335;
        }

        .pros h3, .cons h3 {
            margin-top: 0;
        }

        .applications {
            background-color: #f1f3f4;
            padding: 20px;
            border-radius: 8px;
        }

        .applications ul {
            padding-left: 20px;
        }

        .applications li {
            margin-bottom: 8px;
        }
    </style>
</head>
<body>

<div class="infographic-container">
    <header>
        <h1>ANÁLISIS DE CLASIFICACIÓN DE IMÁGENES (GATO 🐱 vs. PERRO 🐶)</h1>
        <p>Modelo de Regresión Logística aplicado sobre un Dataset de Imágenes Simuladas</p>
        <div class="integrantes">
            <strong>👥 Integrantes:</strong> 
            <span>➡️ José Yohel Huanca Palomino</span>
            <span>➡️ Grimaldo Huacho Criollo</span>
            <span>➡️ Aldair Fabricio Condori Umpire</span>
            <span>➡️ Hirving Rodrigo Paiva Paredes</span>
        </div>
    </header>

    <div class="content-section">

        <h2>📌 Introducción</h2>
        <div class="highlight">
            La **clasificación binaria** consiste en asignar a cada muestra una de dos categorías posibles.  
            En este caso, el reto es distinguir entre **imágenes de gatos (0)** y **perros (1)** utilizando un modelo matemático sencillo: **Regresión Logística**.
        </div>

        <h2>📖 ¿Qué es la Regresión Logística?</h2>
        <p>La regresión logística es un modelo estadístico que utiliza una función sigmoide para estimar la probabilidad de que una muestra pertenezca a una clase determinada.</p>
        <div class="formula">
            P(Y=1|X) = 1 / (1 + e<sup>-z</sup>)  
            donde z = β₀ + β₁x₁ + β₂x₂ + ... + βₙxₙ
        </div>

        <h2>🖼️ Proceso de Entrenamiento</h2>
        <div class="process-steps">
            <div class="step">
                <h4>1️⃣ Dataset</h4>
                <p>Imágenes simuladas de gatos y perros con tamaño <strong>64x64</strong> pixeles.</p>
            </div>
            <div class="step">
                <h4>2️⃣ Preprocesamiento</h4>
                <p>Se aplanan las imágenes en vectores de <strong>4096</strong> características.</p>
            </div>
            <div class="step">
                <h4>3️⃣ Entrenamiento</h4>
                <p>El modelo aprende ajustando pesos (β) mediante máxima verosimilitud.</p>
            </div>
            <div class="step">
                <h4>4️⃣ Predicción</h4>
                <p>Se aplica la función sigmoide para clasificar nuevas imágenes.</p>
            </div>
            <div class="step">
                <h4>5️⃣ Evaluación</h4>
                <p>Se mide la efectividad con <strong>Accuracy</strong>, <strong>Matriz de Confusión</strong> y <strong>Reporte de Clasificación</strong>.</p>
            </div>
        </div>

        <h2>⚖️ Ventajas y Desventajas</h2>
        <div class="pros-cons">
            <div class="pros">
                <h3>✅ Ventajas</h3>
                <ul>
                    <li>Modelo sencillo y fácil de interpretar.</li>
                    <li>Requiere poco poder computacional.</li>
                    <li>Útil como línea base para problemas de clasificación.</li>
                </ul>
            </div>
            <div class="cons">
                <h3>❌ Desventajas</h3>
                <ul>
                    <li>No captura relaciones no lineales complejas.</li>
                    <li>Limitado para imágenes donde la relación espacial es clave.</li>
                    <li>Propenso al sobreajuste si hay muchas variables (como píxeles).</li>
                </ul>
            </div>
        </div>

        <h2>🌐 Aplicaciones en la Vida Real</h2>
        <div class="applications">
            <ul>
                <li>📧 Detección de correos **spam vs. no spam**.</li>
                <li>🏥 Diagnóstico médico (ej. enfermedad presente o no presente).</li>
                <li>💳 Detección de fraudes en transacciones financieras.</li>
                <li>📷 Clasificación básica de imágenes.</li>
                <li>🗳️ Predicción de resultados en encuestas electorales.</li>
            </ul>
        </div>

    </div>
</div>

</body>
</html>
