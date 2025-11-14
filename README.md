
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Lámpara Inteligente Gamer</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, 
        #F7E7CE 0%, 
        #F7E7CE 45%, 
        #3a3a3a 45%,
        #2d2d2d 55%,
        #1a1a1a 65%,
        #0d0d0d 75%,
        #000000 85%,
        #1a1a1a 100%);
      color: white;
      margin: 0;
      padding: 0;
      min-height: 100vh;
    }
    header {
      background: #000000;
      padding: 20px 10px;
      text-align: center;
      font-size: 1.8rem;
      font-weight: bold;
      color: #00eaff;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5);
      position: relative;
    }
    header::before,
    header::after {
      content: '';
      position: absolute;
      top: 0;
      width: 150px;
      height: 100%;
      background-image: url('lampara1.jpg');
      background-size: cover;
      background-position: center;
      opacity: 0.3;
      filter: blur(2px);
    }
    header::before {
      left: 0;
    }
    header::after {
      right: 0;
    }
    
    /* Responsive Design */
    @media (max-width: 768px) {
      header {
        font-size: 1.3rem;
        padding: 15px 5px;
      }
      header::before,
      header::after {
        width: 60px;
      }
    }
    .container {
      padding: 20px;
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }
    .product {
      background: #1a1a1a;
      padding: 15px;
      border-radius: 10px;
      width: 320px;
      max-width: 100%;
    }
    .product img {
      max-width: 100%;
      height: auto;
      border-radius: 5px;
    }
    .stars {
      font-size: 0.9rem;
      color: gold;
      cursor: pointer;
    }
    .image-box {
      width: 100%;
      height: 200px;
      background: #2f2f2f;
      border: 2px dashed #555;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #777;
      font-size: 0.9rem;
      margin-bottom: 10px;
    }
    button {
      width: 100%;
      padding: 10px;
      background: #00eaff;
      border: none;
      color: black;
      font-weight: bold;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 10px;
    }
    button:hover { background: #02b5c7; }
    
    .btn-secundario {
      background: #555 !important;
      color: white !important;
    }
    .btn-secundario:hover {
      background: #777 !important;
    }
    
    .eco-box {
      margin: 30px 20px;
      background: #1a1a1a;
      padding: 15px;
      border-radius: 10px;
      text-align: center;
    }
    .eco-box img {
      max-width: 100px;
      height: auto;
    }
    .eco-img {
      width: 100px;
      margin-bottom: 10px;
    }
    footer {
      text-align: center;
      margin-top: 20px;
      padding: 10px 15px;
      color: #ccc;
      font-size: 0.8rem;
    }
    footer img {
      max-width: 100%;
      height: auto;
    }
    
    /* Responsive para tablets y móviles */
    @media (max-width: 768px) {
      .container {
        padding: 10px;
      }
      .product {
        width: 100%;
      }
      footer {
        font-size: 0.7rem;
        padding: 10px 10px;
      }
      footer h2 {
        font-size: 1.2rem;
      }
    }
  </style>
</head>
<body>
  <header>Lámpara Inteligente Gamer RGB</header>
  <div class="container">
    <div class="product">
      <div class="stars" onclick="document.getElementById('comentarios').style.display='block'">★★★★★ 4.5 / 5</div>
      <h2>Lámpara RGB Gamer</h2>
      <p>Cambia de color con la música. Perfecta para gamers y cuartos modernos. Luz suave y colores vivos.</p>
      <img src="lampara1.jpg" width="300" height="200" />
      <p><b>Precio:</b> $180.900 COP</p>
      <button>Comprar Ahora</button>
      <button class="btn-secundario" onclick="document.getElementById('historia').style.display='block'; window.scrollTo({top: document.getElementById('historia').offsetTop, behavior: 'smooth'});">Historia y Visión</button>
    </div>
  </div>

  <div id="historia" style="display:none; padding: 40px 20px; background: #2a2a2a;">
    <div style="max-width: 800px; margin: 0 auto;">
      <button onclick="document.getElementById('historia').style.display='none'; window.scrollTo({top: 0, behavior: 'smooth'});" style="margin-bottom: 20px; padding: 10px 20px; background: #00eaff; border: none; color: black; font-weight: bold; border-radius: 5px; cursor: pointer; width: auto;">
        ← Volver al Inicio
      </button>
      
      <h2 style="text-align: center; color: #00eaff; margin-bottom: 30px;">Historia y Visión del Proyecto</h2>
      
      <div style="background: #1a1a1a; padding: 25px; border-radius: 10px; line-height: 1.8; text-align: justify;">
        <h3 style="color: #00eaff; margin-top: 0;">El Sueño</h3>
        <p>Este proyecto de mecatrónica nació de un sueño sencillo pero poderoso: crear una luz capaz de transformarse, de cambiar de color, de intensidad y de vida según el momento. Una luz que no solo iluminara un espacio, sino que expresara emociones.</p>
        
        <h3 style="color: #00eaff; margin-top: 25px;">El Diseño</h3>
        <p>A partir de esa idea, comenzó el diseño de una estructura helicoidal, donde un tubo central y una cinta translúcida permitieran que el color viajara en espiral. En su interior, un sistema de LEDs RGB controlados electrónicamente se encarga de generar transiciones suaves y efectos dinámicos. Gracias a un microcontrolador, la lámpara puede modular su brillo, variar su tonalidad y responder a distintos modos preprogramados, creando un espectáculo visual en movimiento.</p>
        
        <h3 style="color: #00eaff; margin-top: 25px;">La Realidad</h3>
        <p>Lo que empezó como un sueño terminó convirtiéndose en un proyecto real: una lámpara inteligente que combina diseño, electrónica y creatividad, demostrando que la mecatrónica puede convertir la imaginación en luz.</p>
      </div>
    </div>
  </div>

  <div id="comentarios" style="display:none; padding: 40px 20px; background: #2a2a2a;">
    <div style="max-width: 800px; margin: 0 auto;">
      <button onclick="document.getElementById('comentarios').style.display='none'" style="margin-bottom: 20px; padding: 10px 20px; background: #00eaff; border: none; color: black; font-weight: bold; border-radius: 5px; cursor: pointer;">
        ← Volver al Menú Principal
      </button>
      
      <h3 style="text-align: center; color: #00eaff;">Comentarios de Clientes</h3>
      <div id="listaComentarios" style="background: #1a1a1a; padding: 15px; border-radius: 10px; margin-bottom: 20px;">
        <p style="margin: 10px 0;">⭐️⭐️⭐️⭐️⭐️ "Muy bonita, hace mi cuarto gamer super cool"</p>
        <p style="margin: 10px 0;">⭐️⭐️⭐️⭐️ "Brilla muy bien y cambia con la música, la amo"</p>
        <p style="margin: 10px 0;">⭐️⭐️⭐️⭐️⭐️ "No gasta mucha energía y se ve genial"</p>
      </div>
      
      <div style="background: #1a1a1a; padding: 20px; border-radius: 10px;">
        <h4 style="color: #00eaff; margin-top: 0;">Deja tu comentario</h4>
        <form id="formComentario" style="display: flex; flex-direction: column; gap: 15px;">
          <div>
            <label style="display: block; margin-bottom: 5px; color: #ccc;">Nombre:</label>
            <input type="text" id="nombre" placeholder="Tu nombre" style="width: 100%; padding: 10px; border-radius: 5px; border: 1px solid #555; background: #2a2a2a; color: white;" required />
          </div>
          
          <div>
            <label style="display: block; margin-bottom: 5px; color: #ccc;">Calificación:</label>
            <select id="calificacion" style="width: 100%; padding: 10px; border-radius: 5px; border: 1px solid #555; background: #2a2a2a; color: white;" required>
              <option value="">Selecciona...</option>
              <option value="5">⭐️⭐️⭐️⭐️⭐️ (5 estrellas)</option>
              <option value="4">⭐️⭐️⭐️⭐️ (4 estrellas)</option>
              <option value="3">⭐️⭐️⭐️ (3 estrellas)</option>
              <option value="2">⭐️⭐️ (2 estrellas)</option>
              <option value="1">⭐️ (1 estrella)</option>
            </select>
          </div>
          
          <div>
            <label style="display: block; margin-bottom: 5px; color: #ccc;">Comentario:</label>
            <textarea id="comentarioTexto" placeholder="Escribe tu opinión sobre el producto..." style="width: 100%; padding: 10px; border-radius: 5px; border: 1px solid #555; background: #2a2a2a; color: white; min-height: 100px; resize: vertical;" required></textarea>
          </div>
          
          <button type="submit" style="width: 100%; padding: 12px; background: #00eaff; border: none; color: black; font-weight: bold; border-radius: 5px; cursor: pointer;">
            Publicar Comentario
          </button>
        </form>
        <div id="mensajeExito" style="display: none; margin-top: 15px; padding: 10px; background: #00eaff; color: black; border-radius: 5px; text-align: center; font-weight: bold;">
          ¡Gracias por tu comentario!
        </div>
      </div>
    </div>
  </div>

  <script>
    document.getElementById('formComentario').addEventListener('submit', function(e) {
      e.preventDefault();
      const nombre = document.getElementById('nombre').value;
      const calificacion = document.getElementById('calificacion').value;
      const comentario = document.getElementById('comentarioTexto').value;
      
      // Crear las estrellas según la calificación
      let estrellas = '';
      for (let i = 0; i < calificacion; i++) {
        estrellas += '⭐️';
      }
      
      // Crear el nuevo comentario
      const nuevoComentario = document.createElement('p');
      nuevoComentario.style.margin = '10px 0';
      nuevoComentario.style.borderLeft = '3px solid #00eaff';
      nuevoComentario.style.paddingLeft = '10px';
      nuevoComentario.innerHTML = `${estrellas} <strong style="color: #00eaff;">${nombre}:</strong> "${comentario}"`;
      
      // Agregar el comentario al inicio de la lista
      const listaComentarios = document.getElementById('listaComentarios');
      listaComentarios.insertBefore(nuevoComentario, listaComentarios.firstChild);
      
      // Mostrar mensaje de éxito
      document.getElementById('mensajeExito').style.display = 'block';
      
      // Limpiar formulario
      this.reset();
      
      // Scroll suave hacia los comentarios
      listaComentarios.scrollIntoView({ behavior: 'smooth', block: 'start' });
      
      // Ocultar mensaje después de 5 minutos (300000 milisegundos)
      setTimeout(() => {
        document.getElementById('mensajeExito').style.display = 'none';
      }, 300000);
    });
  </script>
  <div class="eco-box">
    <img src= "logo1.jpg" width="100" height="100" />
    <p>Esta lámpara cuida el planeta. Es de bajo consumo y tiene certificación Eco+.</p>
  </div>
  <footer>
    Laura Sofía Chacón • Carlos Gómez • Miguel Hernández • Karol Riaño • Cesar Santiago Guasca • Beiker Nivia • Matías Toscano
  <div style="margin-top:40px;text-align:center;">
  <h2>Próximamente</h2>
  <img src="lampara2.jpg" width="400" height="400" />
</div>
</footer>
</body>
</html>
