<!doctype html>
<html lang="es">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Presentación del Equipo PIXES</title>
<style>
  body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(to right, #4f46e5, #06b6d4);
    color: #333;
  }
  header {
    background: rgba(0,0,0,0.7);
    color: white;
    text-align: center;
    padding: 30px;
  }
  header h1 {
    margin: 0;
    font-size: 32px;
  }
  header p {
    margin-top: 8px;
    font-size: 18px;
  }
  .intro {
    background: #fff;
    margin: 20px auto;
    max-width: 900px;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  }
  .intro h2 {
    text-align: center;
    color: #4f46e5;
  }
  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    padding: 20px;
    max-width: 1000px;
    margin: auto;
  }
  .card {
    background: white;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.15);
    text-align: center;
    padding: 15px;
    transition: transform 0.3s;
  }
  .card:hover {
    transform: translateY(-5px);
  }
  .card img {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    object-fit: cover;
    margin-bottom: 10px;
    border: 3px solid #4f46e5;
  }
  .name {
    font-weight: bold;
    font-size: 18px;
    margin: 10px 0 5px;
  }
  .role {
    color: #666;
    font-size: 14px;
    margin-bottom: 8px;
  }
  .hobbies {
    font-size: 12px;
    color: #888;
    margin-top: 5px;
  }
  footer {
    text-align: center;
    background: rgba(0,0,0,0.7);
    color: white;
    padding: 15px;
    margin-top: 30px;
    font-size: 14px;
  }
</style>
</head>
<body>
<header>
  <h1>Equipo de Trabajo — PIXES</h1>
  <p>Unidos por la innovación, el esfuerzo y la creatividad</p>
</header>

<section class="intro">
  <h2>Presentación</h2>
  <p>
    Somos el equipo <strong>PIXES</strong>, conformado por cinco integrantes apasionados 
    por la tecnología, el diseño y la gestión de proyectos. Nuestra misión es 
    desarrollar soluciones innovadoras que aporten valor a los usuarios y 
    mejoren su experiencia en el entorno digital.
  </p>
  <p>
    Como equipo, nos enfocamos en la colaboración, la responsabilidad compartida y 
    el aprendizaje constante. Cada miembro cumple un rol clave, aportando desde 
    su especialidad para lograr un resultado conjunto de calidad.
  </p>
</section>

<section class="grid">
  <!-- Miembro 1 -->
  <div class="card">
    <img src="img/grimaldo.jpg" alt="Grimaldo">
    <div class="name">Grimaldo</div>
    <div class="role">Líder de Proyecto</div>
    <div class="hobbies">Hobbies: Fotografía, Senderismo</div>
  </div>

  <!-- Miembro 2 -->
  <div class="card">
    <img src="img/jose.jpg" alt="Jose Yohel">
    <div class="name">Jose Yohel</div>
    <div class="role">Desarrollador Frontend</div>
    <div class="hobbies">Hobbies: Videojuegos, Ciclismo</div>
  </div>

  <!-- Miembro 3 -->
  <div class="card">
    <img src="img/irving.jpg" alt="Irving">
    <div class="name">Irving</div>
    <div class="role">Diseñador UX/UI</div>
    <div class="hobbies">Hobbies: Dibujo, Música</div>
  </div>

  <!-- Miembro 4 -->
  <div class="card">
    <img src="img/aldair.jpg" alt="Aldair Fabricio">
    <div class="name">Aldair Fabricio</div>
    <div class="role">Administrador de Base de Datos</div>
    <div class="hobbies">Hobbies: Programación, Juegos de Mesa</div>
  </div>

  <!-- Miembro 5 -->
  <div class="card">
    <img src="img/david.jpg" alt="David">
    <div class="name">David</div>
    <div class="role">Coordinador de Comunicación</div>
    <div class="hobbies">Hobbies: Lectura, Fotografía</div>
  </div>
</section>

<footer>
  <p>&copy; 2025 — Equipo PIXES. Todos los derechos reservados.</p>
</footer>
</body>
</html>
