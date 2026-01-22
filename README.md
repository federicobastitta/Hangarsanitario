<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>ALFA SKY | Propuesta de Desarrollo</title>

<style>
  :root{
    --bg:#f4f6f9;
    --text:#0f172a;
    --brand:#0b1220;
    --blue1:#0f1f3d;
    --blue2:#1c4fd8;
    --accent:#1d4ed8;
    --border:#e5e7eb;
    --muted:#cbd5e1;
  }

  *{ box-sizing:border-box; }

  body{
    margin:0;
    font-family: Arial, Helvetica, sans-serif;
    background:var(--bg);
    color:var(--text);
  }

  .container{
    width:min(1100px, calc(100% - 24px));
    margin:16px auto;
    background:#ffffff;
    border-radius:18px;
    box-shadow:0 10px 30px rgba(0,0,0,0.12);
    overflow:hidden;
  }

  /* Barra de marca */
  .brandbar{
    background:var(--brand);
    padding:14px 18px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:12px;
  }
  .brandbar img{
    height:44px;
    width:auto;
    max-width:65%;
    display:block;
  }
  .brandbar .tag{
    color:var(--muted);
    font-size:12px;
    letter-spacing:.2px;
    opacity:.92;
    text-align:right;
    line-height:1.35;
    white-space:nowrap;
  }

  /* Carátula */
  .hero img{
    width:100%;
    height:auto;
    display:block;
  }

  /* Encabezado */
  .header{
    padding:22px 18px;
    background:linear-gradient(135deg,var(--blue1),var(--blue2));
    color:#fff;
  }
  .header h1{
    margin:0;
    font-size:28px;
    letter-spacing:.2px;
    line-height:1.15;
  }
  .header p{
    margin:10px 0 0;
    opacity:.95;
    font-size:15px;
    line-height:1.35;
  }

  /* Secciones */
  .section{
    padding:22px 18px;
    border-bottom:1px solid var(--border);
  }
  .section h2{
    margin:0 0 10px;
    font-size:20px;
    color:var(--accent);
    line-height:1.2;
  }
  .section p{
    margin:10px 0;
    line-height:1.7;
    font-size:15px;
  }
  .bullets{
    margin:10px 0 0;
    padding-left:18px;
  }
  .bullets li{
    margin:8px 0;
    line-height:1.6;
    font-size:15px;
  }

  /* Firma */
  .signature{
    background:var(--brand);
    color:#ffffff;
    padding:26px 18px;
  }
  .signature h2{
    margin:0;
    color:#ffffff;
    font-size:20px;
  }
  .signature-block{
    display:flex;
    flex-wrap:wrap;
    gap:18px;
    margin-top:18px;
  }
  .signature-card{
    flex:1 1 260px;
    min-width:240px;
    padding:14px 14px;
    border:1px solid rgba(255,255,255,0.12);
    border-radius:14px;
    background:rgba(255,255,255,0.04);
  }
  .signature-card strong{
    display:block;
    font-size:17px;
    margin-bottom:6px;
  }
  .signature-card p{
    margin:4px 0 0;
    opacity:.85;
    font-size:14px;
    line-height:1.4;
  }
  .signature-card .pc{
    opacity:.7;
    font-size:13px;
    margin-top:6px;
  }

  /* Footer */
  .footer{
    padding:18px 16px;
    text-align:center;
    color:#64748b;
    font-size:12.5px;
    letter-spacing:.2px;
  }

  /* ====== Breakpoints (tablet/desktop) ====== */
  @media (min-width: 640px){
    .container{ margin:22px auto; }
    .brandbar{ padding:16px 22px; }
    .brandbar img{ height:46px; max-width:70%; }
    .brandbar .tag{ font-size:13px; }
    .header{ padding:26px 22px; }
    .header h1{ font-size:32px; }
    .header p{ font-size:16px; }
    .section{ padding:26px 22px; }
    .section h2{ font-size:22px; }
    .section p, .bullets li{ font-size:15.5px; }
    .signature{ padding:32px 22px; }
    .signature h2{ font-size:22px; }
  }

  @media (min-width: 900px){
    .brandbar{ padding:18px 26px; }
    .header{ padding:28px 26px; }
    .section{ padding:32px 26px; }
    .header h1{ font-size:34px; }
    .signature{ padding:40px 26px; }
  }

  /* Extra: tag no se rompe en móvil chico */
  @media (max-width: 420px){
    .brandbar{
      flex-direction:column;
      align-items:flex-start;
    }
    .brandbar img{
      max-width:100%;
    }
    .brandbar .tag{
      text-align:left;
      white-space:normal;
    }
  }
</style>
</head>

<body>
<div class="container">

  <!-- LOGO -->
  <div class="brandbar">
    <img src="https://raw.githubusercontent.com/federicobastitta/Hangarsanitario/refs/heads/main/logo%20colores%20de%20la%20pagina.png"
         alt="ALFA SKY Logo">
    <div class="tag">
      Propuesta institucional<br>
      Aeroparque Jorge Newbery
    </div>
  </div>

  <!-- PORTADA: FOTO DEL HANGAR MÉDICO -->
  <div class="hero">
    <img src="https://raw.githubusercontent.com/federicobastitta/Hangarsanitario/refs/heads/main/aeropuertos22.png"
         alt="Hangar sanitario - Aeroparque Jorge Newbery">
  </div>

  <!-- TÍTULO -->
  <div class="header">
    <h1>PROPUESTA DE DESARROLLO</h1>
    <p>Servicio de Vuelos Sanitarios desde Aeroparque Jorge Newbery</p>
  </div>

  <!-- 1 -->
  <div class="section">
    <h2>1. Introducción</h2>
    <p>
      Flight Edge S.A.S. (CUIT 33-71647526-9), operando comercialmente bajo el nombre
      ALFA SKY, propone el desarrollo de un servicio aéreo sanitario con base operativa
      en Aeroparque Jorge Newbery, orientado a traslados médicos de alta complejidad,
      derivaciones críticas, evacuaciones sanitarias y vuelos sanitarios programados.
    </p>
    <p>
      El proyecto apunta a cubrir una necesidad real del sistema de salud argentino mediante
      un servicio que actualmente no se encuentra desarrollado en Aeroparque,
      incorporando una prestación de alto impacto sanitario, operativo e institucional.
    </p>
  </div>

  <!-- 2 -->
  <div class="section">
    <h2>2. Ventaja estratégica de Aeroparque</h2>
    <p>
      Aeroparque Jorge Newbery posee una ventaja diferencial única en el país, que lo
      posiciona naturalmente como base de operaciones para vuelos sanitarios:
    </p>
    <ul class="bullets">
      <li>Es el aeropuerto más cercano a los principales hospitales, sanatorios y centros de alta complejidad del Área Metropolitana de Buenos Aires.</li>
      <li>Permite reducir de manera significativa los tiempos críticos de traslado, factor determinante en situaciones médicas complejas.</li>
      <li>Facilita la articulación directa con ambulancias, efectores de salud y sistemas de derivación, tanto públicos como privados.</li>
    </ul>
    <p>
      Estas condiciones convierten a Aeroparque en el hub sanitario aéreo natural de la
      Argentina, una oportunidad estratégica que hoy no se encuentra explotada.
    </p>
  </div>

  <!-- 3 -->
  <div class="section">
    <h2>3. Propuesta de valor</h2>
    <p>
      El proyecto propone que Aeroparque incorpore un servicio aéreo sanitario exclusivo,
      inexistente hasta el momento, que aporte:
    </p>
    <ul class="bullets">
      <li>Una prestación diferencial dentro de la red aeroportuaria nacional.</li>
      <li>Mejora concreta en la capacidad de respuesta ante emergencias médicas y derivaciones complejas.</li>
      <li>Valor institucional y reputacional, al incorporar un servicio directamente vinculado a la salud, alineado con criterios de innovación y responsabilidad social.</li>
      <li>Apertura de un nuevo vertical de negocio, con potencial de crecimiento sostenido.</li>
    </ul>
  </div>

  <!-- 4 -->
  <div class="section">
    <h2>4. Idoneidad y origen del proyecto</h2>
    <p>
      ALFA SKY es una iniciativa impulsada por fundadores con amplia trayectoria en el
      ámbito de la salud, lo que aporta una comprensión profunda de la lógica médica,
      asistencial y operativa.
    </p>
    <p>
      Este origen permite diseñar el servicio no solo desde una perspectiva aeronáutica, sino
      como un sistema integral de traslado sanitario, contemplando tiempos críticos,
      coordinación clínica, protocolos médicos y necesidades reales de los efectores de salud.
    </p>
  </div>

  <!-- 5 -->
  <div class="section">
    <h2>5. Modelo de vinculación con Aeropuertos Argentina 2000</h2>
    <p>
      El objetivo del proyecto es que Aeropuertos Argentina 2000 no sea únicamente un
      proveedor de espacio, sino un actor estratégico del desarrollo.
    </p>
    <p>Se proponen distintas alternativas abiertas, a definir en conjunto:</p>
    <ul class="bullets">
      <li>Asociación estratégica o participación en el negocio.</li>
      <li>Esquemas de revenue sharing por operación.</li>
      <li>Desarrollo conjunto del servicio como prestación distintiva del aeropuerto.</li>
      <li>Cesión y desarrollo de un hangar específico con integración institucional.</li>
    </ul>
    <p>
      La propuesta prioriza una vinculación de largo plazo, alineada con los intereses
      estratégicos de ambas partes.
    </p>
  </div>

  <!-- 6 -->
  <div class="section">
    <h2>6. Alternativa operativa</h2>
    <p>
      Como alternativa técnica, ALFA SKY podría desarrollar el servicio de manera autónoma
      mediante un hangar propio en Aeroparque.
    </p>
    <p>
      Sin perjuicio de ello, se considera claramente superior la opción de vinculación directa
      con Aeropuertos Argentina 2000, por su escala, proyección institucional, legitimidad y
      sinergia estratégica.
    </p>
  </div>

  <!-- 7 -->
  <div class="section">
    <h2>7. Cierre</h2>
    <p>
      El proyecto permite posicionar a Aeroparque Jorge Newbery como un actor central del
      sistema sanitario nacional, incorporando un servicio aéreo crítico hoy inexistente.
    </p>
    <p>
      ALFA SKY aporta el know-how sanitario y operativo; Aeropuertos Argentina 2000, la
      infraestructura, la visión estratégica y el respaldo institucional.
    </p>
    <p>
      La integración de ambos posibilitaría la creación de un modelo único en el país,
      con impacto real en la salud y alto valor estratégico.
    </p>
  </div>

  <!-- FIRMA -->
  <div class="signature">
    <h2>Firma Institucional</h2>
    <div class="signature-block">
      <div class="signature-card">
        <strong>Dr. Federico Bastitta</strong>
        <p>CEO · ALFA SKY</p>
      </div>
      <div class="signature-card">
        <strong>Ariel Evasio</strong>
        <p>CEO · ALFA SKY</p>
        <p class="pc">PC</p>
      </div>
    </div>
  </div>

  <div class="footer">
    Documento institucional — Propuesta de desarrollo estratégico
  </div>

</div>
</body>
</html>

