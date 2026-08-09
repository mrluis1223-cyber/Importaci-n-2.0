<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Bitácora de Ruta — Itsmo Cars</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Oswald:wght@500;600;700&family=IBM+Plex+Sans:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --navy-deep:#0D1B2A; --navy-panel:#16283D; --navy-panel-2:#1C3350;
    --brass:#C89B4A; --stamp-red:#C44536; --transit-teal:#3E8E8A;
    --cream:#EDE6D6; --muted:#8FA3B8; --line:#2A4360;
  }
  *{box-sizing:border-box;}
  body{
    margin:0; background:var(--navy-deep);
    background-image:radial-gradient(circle at 8% 0%, rgba(200,155,74,0.07), transparent 40%),
      radial-gradient(circle at 92% 100%, rgba(196,69,54,0.05), transparent 40%);
    color:var(--cream); font-family:'IBM Plex Sans', sans-serif; padding:32px 16px 80px;
  }
  .wrap{max-width:820px; margin:0 auto;}

  .manifest{ border:1px solid var(--line); border-radius:4px; background:var(--navy-panel);
    padding:26px 24px; position:relative; overflow:hidden; opacity:0; animation: simpleFade .7s ease forwards; }
  @keyframes simpleFade{ to{opacity:1;} }
  .manifest::before{ content:""; position:absolute; top:0; left:0; right:0; height:3px;
    background:repeating-linear-gradient(90deg, var(--brass) 0 14px, transparent 14px 22px); opacity:.6; }
  .eyebrow{ font-family:'IBM Plex Mono', monospace; font-size:11px; letter-spacing:.18em;
    color:var(--brass); text-transform:uppercase; margin-bottom:8px; }
  h1{ font-family:'Oswald', sans-serif; font-weight:700; font-size:clamp(24px,5vw,34px);
    text-transform:uppercase; margin:0 0 14px; line-height:1.05; }
  .meta-grid{ display:grid; grid-template-columns:repeat(2,1fr); gap:12px 22px;
    border-top:1px dashed var(--line); padding-top:16px; }
  .meta-item .label{ font-family:'IBM Plex Mono', monospace; font-size:10px; letter-spacing:.09em;
    text-transform:uppercase; color:var(--muted); margin-bottom:2px; }
  .meta-item .value{font-size:13.5px; font-weight:500;}

  .route-section{ margin-top:26px; border:1px solid var(--line); border-radius:4px;
    background:var(--navy-panel); padding:18px; opacity:0; animation: simpleFade .7s ease .15s forwards; overflow:hidden; }
  .route-title{ font-family:'Oswald', sans-serif; text-transform:uppercase; font-size:14px;
    letter-spacing:.08em; color:var(--brass); margin:0 0 14px; }
  .route-video{ width:100%; border-radius:4px; display:block; border:1px solid var(--line); }
  .avoided{ display:flex; align-items:center; gap:8px; font-family:'IBM Plex Mono', monospace;
    font-size:11px; color:var(--stamp-red); margin:14px 0 4px; opacity:.85; }
  .avoided .strike{ text-decoration: line-through; text-decoration-color: var(--stamp-red); }
  .route-footnote{ font-size:12px; color:var(--muted); line-height:1.6; border-top:1px dashed var(--line);
    padding-top:12px; margin-top:10px; }
  .route-footnote strong{color:var(--cream);}

  .timeline{ margin-top:30px; position:relative; padding-left:34px; }
  .timeline::before{ content:""; position:absolute; left:11px; top:6px; bottom:6px; width:2px;
    background:repeating-linear-gradient(to bottom, var(--line) 0 6px, transparent 6px 11px); }
  .stop{ position:relative; padding-bottom:26px; }
  .stop:last-child{padding-bottom:0;}
  .node{ position:absolute; left:-34px; top:2px; width:24px; height:24px; border-radius:50%;
    background:var(--navy-panel-2); border:2px solid var(--brass); display:flex; align-items:center;
    justify-content:center; font-family:'IBM Plex Mono', monospace; font-size:10px; font-weight:600;
    color:var(--brass); opacity:0; }
  .stop.visible .node{ animation: nodePop .35s steps(4) forwards; }
  @keyframes nodePop{ 0%{opacity:0; transform:scale(.4);} 100%{opacity:1; transform:scale(1);} }
  .stop.customs .node{border-color:var(--stamp-red); color:var(--stamp-red);}
  .stop.transitfiscal .node{border-color:var(--transit-teal); color:var(--transit-teal);}

  .card{ background:var(--navy-panel); border:1px solid var(--line); border-radius:4px;
    padding:0; opacity:0; transform:translateY(-14px); overflow:hidden;
    display:flex; flex-wrap:wrap; }
  .stop.visible .card{ animation: cardIn .4s steps(4) forwards; }
  @keyframes cardIn{ to{ opacity:1; transform:translateY(0); } }
  .stop.customs .card{border-left:3px solid var(--stamp-red);}
  .stop.transitfiscal .card{border-left:3px solid var(--transit-teal);}

  .clip{ flex:0 0 200px; width:200px; height:140px; background:#000; }
  .clip video{ width:100%; height:100%; object-fit:cover; display:block; }

  .card-body{ flex:1 1 240px; min-width:0; padding:13px 16px; }
  .card-top{ display:flex; justify-content:space-between; align-items:baseline; gap:10px; margin-bottom:4px; flex-wrap:wrap; }
  .step-num{ font-family:'IBM Plex Mono', monospace; font-size:10px; color:var(--brass); letter-spacing:.08em; }
  .stop.customs .step-num{color:var(--stamp-red);}
  .stop.transitfiscal .step-num{color:var(--transit-teal);}
  .scope{ font-size:11.5px; font-style:italic; color:var(--brass); opacity:.85; margin-bottom:6px; line-height:1.4; }
  .stop.customs .scope{ color:#e08276; }
  .stop.transitfiscal .scope{ color:#79c4c0; }
  .actor{ font-family:'Oswald', sans-serif; font-size:15px; font-weight:600; text-transform:uppercase; }
  .desc{ font-size:12.5px; color:var(--muted); margin:2px 0 8px; line-height:1.45; }
  .tags{ display:flex; flex-wrap:wrap; gap:6px; }
  .doc-tag{ display:inline-flex; align-items:center; gap:5px; font-family:'IBM Plex Mono', monospace;
    font-size:10.5px; color:var(--cream); background:rgba(200,155,74,0.12);
    border:1px solid rgba(200,155,74,0.35); padding:3px 8px; border-radius:2px; }
  .stop.customs .doc-tag{ background:rgba(196,69,54,0.12); border-color:rgba(196,69,54,0.35); }
  .stop.transitfiscal .doc-tag{ background:rgba(62,142,138,0.14); border-color:rgba(62,142,138,0.4); }

  .tax-box{ margin-top:30px; border:1px solid var(--line); border-radius:4px; background:var(--navy-panel);
    padding:20px; opacity:0; }
  .tax-box.visible{ animation: simpleFade .6s ease forwards; }
  .tax-box h2{ font-family:'Oswald', sans-serif; text-transform:uppercase; font-size:15px;
    letter-spacing:.06em; color:var(--brass); margin:0 0 14px; }
  table{ width:100%; border-collapse:collapse; font-size:12.5px; }
  th,td{ text-align:left; padding:6px 4px; border-bottom:1px solid var(--line); }
  th{ font-family:'IBM Plex Mono', monospace; font-size:10px; text-transform:uppercase; color:var(--muted); font-weight:500; }
  td.num{ text-align:right; font-family:'IBM Plex Mono', monospace; }
  tr.total td{ color:var(--brass); font-weight:600; border-top:1px solid var(--brass); border-bottom:none; padding-top:9px; }

  .footer-note{ margin-top:30px; border-top:1px dashed var(--line); padding-top:16px;
    font-size:12px; color:var(--muted); line-height:1.7; }
  .footer-note strong{color:var(--cream);}
  .hint{ text-align:center; font-family:'IBM Plex Mono', monospace; font-size:10.5px; color:var(--muted);
    margin-top:10px; letter-spacing:.06em; }

  @media(max-width:560px){
    .meta-grid{grid-template-columns:1fr;}
    .clip{ flex:1 1 100%; width:100%; height:180px; }
    .card-body{ flex:1 1 100%; }
  }
</style>
</head>
<body>
<div class="wrap">

  <div class="manifest">
    <div class="eyebrow">Bitácora de Ruta · Escenario Logístico Completo</div>
    <h1>Importación de Vehículos — Itsmo Cars</h1>
    <div class="meta-grid">
      <div class="meta-item"><div class="label">Mercancía</div><div class="value">3x Toyota Land Cruiser 79, DC, 4.5L V8 TD, 0km</div></div>
      <div class="meta-item"><div class="label">Clasificación</div><div class="value">Partida 8704.21.00.00.00</div></div>
      <div class="meta-item"><div class="label">Incoterm</div><div class="value">CIF (flete y seguro incluidos)</div></div>
      <div class="meta-item"><div class="label">Modalidad</div><div class="value">RoRo</div></div>
      <div class="meta-item"><div class="label">Exportador</div><div class="value">Al-Rashid Motors Trading Co. — Jeddah</div></div>
      <div class="meta-item"><div class="label">Importador</div><div class="value">Itsmo Cars — Altaplaza, Panamá</div></div>
      <div class="meta-item"><div class="label">Valor CIF total</div><div class="value">US$150,000 (US$50,000/unidad)</div></div>
      <div class="meta-item"><div class="label">Régimen aduanero</div><div class="value">Tránsito hacia Recinto Fiscal propio</div></div>
    </div>
  </div>

  <div class="route-section">
    <div class="route-title">Ruta marítima internacional</div>
    <video class="route-video" autoplay muted loop playsinline>
      <source src="videos/ruta_mapa.mp4" type="video/mp4">
    </video>
    <div class="avoided">⚠ <span class="strike">Vía Canal de Suez / Mar Rojo</span> — evitada por advertencia Houthi vigente contra buques vinculados a Arabia Saudita (desde 20 jul. 2026)</div>
    <div class="route-footnote"><strong>Naviera:</strong> Wallenius Wilhelmsen (PCTC) · <strong>Seguro:</strong> MedGulf — ICC(A) + War Risk, póliza PA-CARGO-MG-2026-77410</div>
  </div>

  <div class="hint">↓ desliza para ver la bitácora completa ↓</div>

  <div class="timeline">

    <div class="stop">
      <div class="node">01</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e01_partes.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">01 · PARTES CONTRATANTES</span></div>
          <div class="scope">Qué abarca: define quiénes son las partes, qué se compra, bajo qué Incoterm y qué modalidad de transporte.</div>
          <div class="actor">Al-Rashid Motors ↔ Itsmo Cars</div>
          <div class="desc">Jeddah → Altaplaza, Panamá. CIF, RoRo, 3 unidades 0km.</div>
        </div>
      </div>
    </div>

    <div class="stop">
      <div class="node">02</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e02_negociacion.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">02 · NEGOCIACIÓN COMERCIAL</span></div>
          <div class="scope">Qué abarca: fija el precio final pactado, base de todos los cálculos de impuestos posteriores.</div>
          <div class="actor">Acuerdo de precio (videollamada)</div>
          <div class="desc">US$68,000 → negociado a US$50,000 CIF/unidad.</div>
          <div class="tags"><span class="doc-tag">PI-2026-0417</span></div>
        </div>
      </div>
    </div>

    <div class="stop">
      <div class="node">03</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e03_preparacion.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">03 · PREPARACIÓN DE MERCANCÍA</span></div>
          <div class="scope">Qué abarca: verifica estado físico y documental del vehículo antes de salir del país de origen.</div>
          <div class="actor">SGS Arabia Saudita</div>
          <div class="desc">Inspección VIN/estado, motor y checklist por unidad. COC Toyota Arabia Saudita.</div>
          <div class="tags"><span class="doc-tag">SGS-JED-2026-00317</span></div>
        </div>
      </div>
    </div>

    <div class="stop">
      <div class="node">04</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e04_logistica.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">04 · LOGÍSTICA EN ORIGEN</span></div>
          <div class="scope">Qué abarca: organiza el traslado interno y reserva el espacio en el buque.</div>
          <div class="actor">Hejaz Cargo Forwarding Co.</div>
          <div class="desc">Carga en portavehículos y traslado a Terminal RoRo de Jeddah.</div>
          <div class="tags"><span class="doc-tag">Booking WWL-SA-88452</span></div>
        </div>
      </div>
    </div>

    <div class="stop customs">
      <div class="node">05</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e05_aduana_export.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">05 · ADUANA DE EXPORTACIÓN</span></div>
          <div class="scope">Qué abarca: formaliza la salida legal de la mercancía ante las autoridades sauditas.</div>
          <div class="actor">JIT-Ex Customs Clearance</div>
          <div class="desc">Declaración ZATCA. Certificado de origen (Cámara de Comercio Jeddah).</div>
          <div class="tags"><span class="doc-tag">EXP-2026-119045</span><span class="doc-tag">CO-SA-2026-0089</span></div>
        </div>
      </div>
    </div>

    <div class="stop">
      <div class="node">06</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e06_embarque.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">06 · PUERTO DE ORIGEN Y EMBARQUE</span></div>
          <div class="scope">Qué abarca: carga física a bordo del buque y emisión del documento de transporte marítimo.</div>
          <div class="actor">Jeddah Islamic Port · Mawani</div>
          <div class="desc">Carga RoRo "drive-on" al buque PCTC de WWL.</div>
          <div class="tags"><span class="doc-tag">B/L WWL-JED-CRI-2026-30187</span></div>
        </div>
      </div>
    </div>

    <div class="stop">
      <div class="node">07</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e07_transito.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">07 · TRÁNSITO INTERNACIONAL</span></div>
          <div class="scope">Qué abarca: el trayecto marítimo entre origen y destino, con cobertura de seguro activa.</div>
          <div class="actor">Ruta Cabo de Buena Esperanza</div>
          <div class="desc">~13,000 mn, ~40-45 días. Evita Mar Rojo/Suez por riesgo Houthi vigente.</div>
          <div class="tags"><span class="doc-tag">Póliza PA-CARGO-MG-2026-77410</span></div>
        </div>
      </div>
    </div>

    <div class="stop">
      <div class="node">08</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e08_descarga.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">08 · PUERTO DE DESTINO Y DESCARGA</span></div>
          <div class="scope">Qué abarca: recepción y descarga de la mercancía en el puerto panameño.</div>
          <div class="actor">Manzanillo International Terminal</div>
          <div class="desc">Coco Solo, Colón. Operado por SSA Marine. Descarga "drive-off".</div>
          <div class="tags"><span class="doc-tag">Discharge Report</span></div>
        </div>
      </div>
    </div>

    <div class="stop customs">
      <div class="node">09</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e09_transito_aduanero.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">09 · TRÁNSITO ADUANERO INTERNO</span></div>
          <div class="scope">Qué abarca: mueve la mercancía sin nacionalizar hasta el recinto fiscal, bajo garantía y sin pago inmediato.</div>
          <div class="actor">Grupo Aduanero Kam</div>
          <div class="desc">Salida de MIT y traslado hasta el Recinto Fiscal Aduanero. Garantía por US$25,500.</div>
          <div class="tags"><span class="doc-tag">DTA-2026-PA-004521</span></div>
        </div>
      </div>
    </div>

    <div class="stop transitfiscal">
      <div class="node">10</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e10_recinto_fiscal.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">10 · TRANSPORTE A RECINTO FISCAL</span></div>
          <div class="scope">Qué abarca: traslado bajo control y precinto aduanero hasta la bodega autorizada.</div>
          <div class="actor">MACS Marine Transport</div>
          <div class="desc">Llegada a bodega de Itsmo Cars, Vía Ricardo J. Alfaro, Altaplaza.</div>
          <div class="tags"><span class="doc-tag">ARF-2026-4471</span></div>
        </div>
      </div>
    </div>

    <div class="stop customs">
      <div class="node">11</div>
      <div class="card">
        <div class="clip"><video autoplay muted loop playsinline><source src="videos/e11_nacionalizacion.mp4" type="video/mp4"></video></div>
        <div class="card-body">
          <div class="card-top"><span class="step-num">11 · NACIONALIZACIÓN Y ENTREGA FINAL</span></div>
          <div class="scope">Qué abarca: liquida impuestos por unidad según demanda y cierra trámites para poder circular.</div>
          <div class="actor">Itsmo Cars</div>
          <div class="desc">DAI 0% + ISC 10% + ITBMS 7%. Trámites: DIJ, ATTT (matrícula), Municipio.</div>
          <div class="tags"><span class="doc-tag">Título — pendiente ATTT</span></div>
        </div>
      </div>
    </div>

  </div>

  <div class="tax-box" id="taxBox">
    <h2>Carga tributaria — Partida 8704.21.00.00.00</h2>
    <table>
      <tr><th>Concepto</th><th class="num">Tasa</th><th class="num">Monto (3 unid.)</th></tr>
      <tr><td>Valor CIF total</td><td class="num">—</td><td class="num">US$150,000</td></tr>
      <tr><td>DAI</td><td class="num">0%</td><td class="num">US$0</td></tr>
      <tr><td>ISC</td><td class="num">10%</td><td class="num">US$15,000</td></tr>
      <tr><td>ITBMS</td><td class="num">7%</td><td class="num">US$10,500</td></tr>
      <tr><td>ICCDP</td><td class="num">0%</td><td class="num">US$0</td></tr>
      <tr class="total"><td>Valor nacionalizado total</td><td class="num"></td><td class="num">US$175,500</td></tr>
    </table>
  </div>

  <div class="footer-note"><strong>Nota:</strong> videos propios del usuario (stop motion/claymation), cortados y ubicados según la etapa correspondiente. Cifras y clasificación arancelaria reales. Empresas de servicios logísticos son reales; exportador e importador son ficticios. Dirección en Altaplaza es ilustrativa.</div>

</div>

<script>
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) { entry.target.classList.add('visible'); observer.unobserve(entry.target); }
    });
  }, { threshold: 0.2 });
  document.querySelectorAll('.stop').forEach(el => observer.observe(el));
  const taxBox = document.getElementById('taxBox');
  if (taxBox) observer.observe(taxBox);
</script>

</body>
</html>
