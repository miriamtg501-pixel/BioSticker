<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>BioSticker – Dispositivo de monitoreo continuo</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 20px; line-height: 1.6; }
    header { text-align: center; margin-bottom: 40px; }
    .caratula { background: #f0f0f0; padding: 50px 20px; border-radius: 10px; }
    .contenedor { max-width: 800px; margin: auto; }
    img { max-width: 100%; height: auto; }
    .contador { font-size: 1.2em; margin: 20px 0; color: #555; }
    .qr { text-align: center; margin: 30px 0; }
    footer { text-align: center; margin-top: 50px; font-size: 0.9em; color: #888; }
  </style>
</head>
<body>
  <div class="contenedor">
    <!-- CARÁTULA -->
    <header class="caratula">
      <h1>BioSticker</h1>
      <p>Dispositivo médico de monitoreo continuo de signos vitales</p>
      <p>Autor: [Miriam Torres Garcia]</p>
      <p>Fecha: [31 de Octubre 2025]</p>
    </header>

    <!-- CONTADOR DE VISITAS -->
    <div class="contador">
      Visitas a esta página: <span id="visitCount">0</span>
    </div>

    <!-- IMÁGENES DEL DISPOSITIVO -->
    <section>
      <h2>Imágenes del dispositivo</h2>
      <img src="https://www.philips.com/a-w/about/news/media-library/20200709-BioSticker-and-BioHub.html/download/large" alt="BioSticker dispositivo">
      <img src="https://www.bioworld.com/articles/432685-biointellisense-scores-win-at-fda-with-the-clearance-of-its-biosticker/v=preview" alt="BioSticker sobre el cuerpo">
      <img src="https://wearable-technologies.com/news/aloe-care-health-and-biointellisense-partner-up-to-provide-remote-patient-monitoring-to-elderly-adults" alt="BioSticker wearable">
    </section>

    <!-- TEXTO EXPLICATIVO -->
    <section>
      <h2>¿Qué es el BioSticker?</h2>
      <p>El BioSticker es un dispositivo médico portátil de un solo uso que permite <strong>hasta 30 días de monitoreo continuo de signos vitales</strong>, como frecuencia cardíaca, frecuencia respiratoria, temperatura de la piel y otros datos biométricos esenciales. :contentReference[oaicite:2]{index=2}</p>
      <p>Diseñado para ser usado en el torso del paciente (parte superior del pecho), el BioSticker ™ ofrece una experiencia cómoda e integrada para la atención remota. :contentReference[oaicite:3]{index=3}</p>
      <p>Este tipo de tecnología es clave en los modelos de monitoreo remoto de pacientes (RPM), ya que permite que los equipos de salud supervisen condiciones médicas fuera del hospital, mejorando la detección temprana de complicaciones. :contentReference[oaicite:4]{index=4}</p>
    </section>

    <!-- VIDEO -->
    <section>
      <h2>Video demostrativo</h2>
      <iframe width="560" height="315" src="https://www.youtube.com/embed/JVM4f0rCamo" 
        title="Video BioSticker" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
      </iframe>
    </section>

    <!-- CÓDIGO QR DE LA UBICACIÓN ESM -->
    <section class="qr">
      <h2>Ubicación de la Escuela Superior de Medicina (ESM-IPN)</h2>
      <p>Escanea el código QR para ver la ubicación:</p>
      <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=https://maps.google.com/?q=Escuela+Superior+de+Medicina+IPN+Ciudad+de+México" alt="Código QR ESM-IPN">
      <p>Dirección: Salvador Díaz Mirón esq. Plan de San Luis s/n, Col. Casco de Santo Tomás, C.P. 11340, Miguel Hidalgo, Ciudad de México. :contentReference[oaicite:5]{index=5}</p>
    </section>

    <footer>
      Página creada para tarea de Informática Médica.
    </footer>
  </div>

  <script>
    // SCRIPT SIMPLE PARA CONTADOR DE VISITAS (USANDO localStorage)
    const countEl = document.getElementById('visitCount');
    let count = localStorage.getItem('visitCount');
    if (!count) {
      count = 0;
    }
    count++;
    localStorage.setItem('visitCount', count);
    countEl.textContent = count;
  </script>
</body>
</html>
