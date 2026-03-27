<style>
/* ========== RESET & BASE ========== */
body, .markdown-body {
  font-family: 'Poppins', 'Segoe UI', sans-serif;
  background: #f5f8fb;
  color: #182244;
}

/* ========== COVER ========== */
.cover {
  background: linear-gradient(135deg, #002F47 0%, #0182C4 60%, #00D6F9 100%);
  border-radius: 16px;
  padding: 64px 48px;
  text-align: center;
  margin-bottom: 48px;
  position: relative;
  overflow: hidden;
}
.cover::before {
  content: '';
  position: absolute;
  top: -60px; right: -60px;
  width: 260px; height: 260px;
  border-radius: 50%;
  background: rgba(255,255,255,0.06);
}
.cover::after {
  content: '';
  position: absolute;
  bottom: -80px; left: -40px;
  width: 320px; height: 320px;
  border-radius: 50%;
  background: rgba(0,214,249,0.08);
}
.cover h1 {
  color: #fff;
  font-size: 3rem;
  font-weight: 900;
  letter-spacing: 2px;
  margin: 0 0 8px;
  text-shadow: 0 2px 12px rgba(0,0,0,0.25);
}
.cover .subtitle {
  color: #00D6F9;
  font-size: 1.25rem;
  font-weight: 600;
  letter-spacing: 4px;
  text-transform: uppercase;
  margin-bottom: 32px;
}
.cover .year {
  color: rgba(255,255,255,0.5);
  font-size: 0.95rem;
  letter-spacing: 2px;
}

/* ========== TABLE OF CONTENTS ========== */
.toc {
  background: #fff;
  border-left: 6px solid #0182C4;
  border-radius: 0 12px 12px 0;
  padding: 28px 36px;
  margin-bottom: 48px;
  box-shadow: 0 4px 20px rgba(1,130,196,0.08);
}
.toc h2 {
  color: #0182C4;
  font-size: 1.1rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 3px;
  margin-top: 0;
}
.toc ol {
  margin: 0;
  padding-left: 20px;
}
.toc li {
  margin: 8px 0;
  font-weight: 500;
}
.toc a {
  color: #002F47;
  text-decoration: none;
}
.toc a:hover {
  color: #0182C4;
  text-decoration: underline;
}

/* ========== SECTION HEADERS ========== */
.section-header {
  display: flex;
  align-items: center;
  gap: 16px;
  margin: 56px 0 24px;
}
.section-number {
  background: linear-gradient(135deg, #0182C4, #00D6F9);
  color: #fff;
  font-size: 1.5rem;
  font-weight: 900;
  width: 56px; height: 56px;
  border-radius: 50%;
  display: flex; align-items: center; justify-content: center;
  flex-shrink: 0;
  box-shadow: 0 4px 16px rgba(1,130,196,0.3);
}
.section-title {
  font-size: 2rem;
  font-weight: 800;
  color: #002F47;
  letter-spacing: 1px;
}

/* ========== CARDS ========== */
.card {
  background: #fff;
  border-radius: 12px;
  padding: 28px 32px;
  margin-bottom: 24px;
  box-shadow: 0 2px 16px rgba(1,130,196,0.07);
  border: 1px solid #e8f0fa;
}
.card h3 {
  color: #0182C4;
  font-size: 1.1rem;
  font-weight: 700;
  margin-top: 0;
  text-transform: uppercase;
  letter-spacing: 1px;
}

/* ========== LOGO GRID ========== */
.logo-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 20px;
  margin: 24px 0;
}
.logo-card {
  border-radius: 12px;
  padding: 24px;
  text-align: center;
  border: 1.5px solid #e2eaf5;
}
.logo-card.light {
  background: #f0f6fc;
}
.logo-card.dark {
  background: linear-gradient(135deg, #002F47, #0182C4);
}
.logo-card img {
  max-width: 100%;
  max-height: 120px;
  object-fit: contain;
  margin-bottom: 12px;
}
.logo-card .logo-label {
  font-size: 0.82rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 1.5px;
}
.logo-card.light .logo-label { color: #0182C4; }
.logo-card.dark .logo-label  { color: #00D6F9; }

/* ========== SAFETY AREA BOX ========== */
.safety-box {
  background: #fff;
  border: 2px dashed #0182C4;
  border-radius: 12px;
  padding: 28px 32px;
  margin: 20px 0;
  text-align: center;
}
.safety-box p { margin: 4px 0; }

/* ========== SIZE TABLE ========== */
.size-table {
  width: 100%;
  border-collapse: collapse;
  margin: 16px 0;
  font-size: 0.92rem;
}
.size-table th {
  background: #0182C4;
  color: #fff;
  padding: 10px 16px;
  text-align: left;
  font-weight: 600;
}
.size-table td {
  padding: 10px 16px;
  border-bottom: 1px solid #e2eaf5;
}
.size-table tr:nth-child(even) td { background: #f5f8fb; }

/* ========== DO / DON'T ========== */
.do-dont {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
  margin: 20px 0;
}
.do-box, .dont-box {
  border-radius: 10px;
  padding: 20px 24px;
}
.do-box {
  background: #f0faf4;
  border: 2px solid #7EEC90;
}
.dont-box {
  background: #fff5f7;
  border: 2px solid #F5659A;
}
.do-box h4 {
  color: #2a9d4e;
  margin-top: 0;
  font-size: 0.95rem;
  text-transform: uppercase;
  letter-spacing: 1px;
}
.dont-box h4 {
  color: #c0305a;
  margin-top: 0;
  font-size: 0.95rem;
  text-transform: uppercase;
  letter-spacing: 1px;
}
.do-box ul, .dont-box ul {
  margin: 0; padding-left: 18px;
  font-size: 0.9rem;
}
.do-box li { color: #2a9d4e; }
.dont-box li { color: #c0305a; }

/* ========== COBRANDING ========== */
.cobranding-box {
  background: #fff;
  border-left: 5px solid #5A26EE;
  border-radius: 0 12px 12px 0;
  padding: 24px 28px;
  margin: 20px 0;
  box-shadow: 0 2px 12px rgba(90,38,238,0.07);
}
.cobranding-box h4 {
  color: #5A26EE;
  margin-top: 0;
  font-size: 1rem;
  font-weight: 700;
}

/* ========== TYPOGRAPHY ========== */
.type-showcase {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 16px;
  margin: 20px 0;
}
.type-card {
  background: #fff;
  border-radius: 10px;
  padding: 20px 24px;
  border-top: 4px solid #0182C4;
  box-shadow: 0 2px 12px rgba(1,130,196,0.06);
}
.type-card .weight-name {
  font-size: 0.8rem;
  color: #0182C4;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-bottom: 8px;
}
.type-card .sample-text {
  font-size: 1.6rem;
  color: #002F47;
  line-height: 1.2;
}
.type-card .size-range {
  font-size: 0.78rem;
  color: #8a9ab5;
  margin-top: 10px;
}
.type-alphabet {
  background: #f0f6fc;
  border-radius: 10px;
  padding: 20px 24px;
  font-family: 'Poppins', sans-serif;
  font-size: 1.05rem;
  line-height: 2;
  color: #002F47;
  letter-spacing: 1.5px;
  margin: 16px 0;
  text-align: center;
}

/* ========== COLORS ========== */
.color-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 16px;
  margin: 20px 0;
}
.color-chip {
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 2px 12px rgba(0,0,0,0.08);
}
.color-swatch {
  height: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.color-swatch .hex {
  font-size: 1rem;
  font-weight: 700;
  color: rgba(255,255,255,0.9);
  letter-spacing: 1px;
  text-shadow: 0 1px 4px rgba(0,0,0,0.3);
}
.color-info {
  background: #fff;
  padding: 12px 16px;
}
.color-info .color-name {
  font-weight: 700;
  font-size: 0.88rem;
  color: #182244;
}
.color-info .color-role {
  font-size: 0.76rem;
  color: #8a9ab5;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-top: 2px;
}
.color-info .color-meaning {
  font-size: 0.8rem;
  color: #4a5a7a;
  margin-top: 6px;
  font-style: italic;
}

/* ========== INFO BOX ========== */
.info-box {
  background: linear-gradient(135deg, #e8f4fc 0%, #f0eeff 100%);
  border-radius: 10px;
  padding: 18px 24px;
  margin: 16px 0;
  border-left: 4px solid #1389FB;
  font-size: 0.93rem;
  color: #2a3a5a;
}
.info-box strong { color: #0182C4; }

/* ========== PHOTO STYLE ========== */
.photo-style {
  background: linear-gradient(135deg, #002F47 0%, #0182C4 100%);
  border-radius: 12px;
  padding: 32px;
  color: #fff;
  margin: 20px 0;
}
.photo-style h4 {
  color: #00D6F9;
  margin-top: 0;
  font-size: 1.1rem;
  letter-spacing: 1px;
}
.photo-style ul {
  margin: 0; padding-left: 20px;
  line-height: 2;
}

/* ========== APPLICATIONS ========== */
.app-examples {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 16px;
  margin: 20px 0;
}
.app-example {
  background: linear-gradient(135deg, #0182C4 0%, #00D6F9 100%);
  border-radius: 12px;
  padding: 28px;
  color: #fff;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 8px;
}
.app-example .app-name {
  font-size: 0.78rem;
  text-transform: uppercase;
  letter-spacing: 2px;
  color: rgba(255,255,255,0.7);
}
.app-example .app-title {
  font-size: 1.15rem;
  font-weight: 700;
}

/* ========== DIVIDER ========== */
.divider {
  border: none;
  height: 2px;
  background: linear-gradient(90deg, #0182C4, #00D6F9, transparent);
  border-radius: 2px;
  margin: 40px 0;
}

/* ========== FOOTER ========== */
.footer {
  text-align: center;
  padding: 32px;
  background: #002F47;
  border-radius: 12px;
  color: rgba(255,255,255,0.5);
  font-size: 0.82rem;
  letter-spacing: 1px;
  margin-top: 56px;
}
.footer strong { color: #00D6F9; }
</style>

<div class="cover">
  <h1>OlimpIA</h1>
  <div class="subtitle">Manual de Marca</div>
  <img src="Logo OlimpIA - Imágenes/Logo-OlimpIA-Blanco.png" alt="Logo OlimpIA Blanco" style="max-width:260px;margin:24px auto 20px;display:block;filter:drop-shadow(0 4px 16px rgba(0,0,0,0.25))"/>
  <div class="year">© 2024 · Versión 1.0</div>
</div>

---

<div class="toc">
<h2>📋 Contenido</h2>
<ol>
  <li><a href="#01-nuestra-marca">Nuestra Marca</a> — Logo, área de seguridad, versiones, cobranding, aplicaciones incorrectas</li>
  <li><a href="#02-tipografía-corporativa">Tipografía Corporativa</a> — Familia Poppins, jerarquía, tamaños</li>
  <li><a href="#03-color">Color</a> — Colores primarios, complementarios y acentos</li>
  <li><a href="#04-iconografía">Iconografía</a> — Criterios de uso de íconos</li>
  <li><a href="#05-fotografía">Fotografía</a> — Estilo y criterios fotográficos</li>
  <li><a href="#06-aplicaciones">Aplicaciones</a> — Ejemplos de uso de la marca</li>
</ol>
</div>

---

<div class="section-header" id="01-nuestra-marca">
  <div class="section-number">01</div>
  <div class="section-title">Nuestra Marca</div>
</div>

<div class="card">
<h3>Logotipo aprobado</h3>
<p>Este es el logotipo aprobado y usado en todas las comunicaciones de la compañía. Es el activo visual más valioso de OlimpIA y debe utilizarse con exactitud en todas sus versiones.</p>
</div>

### Versiones del logotipo

<div class="logo-grid">
  <div class="logo-card light">
    <img src="Logo OlimpIA - Imágenes/Logo-OlimpIA-Color.png" alt="Logo OlimpIA Color - Versión horizontal"/>
    <div class="logo-label">Versión horizontal — Color</div>
  </div>
  <div class="logo-card dark">
    <img src="Logo OlimpIA - Imágenes/Logo-OlimpIA-Blanco.png" alt="Logo OlimpIA Blanco - Versión horizontal"/>
    <div class="logo-label">Versión horizontal — Blanco</div>
  </div>
  <div class="logo-card light">
    <img src="Logo OlimpIA - Imágenes/Logo-OlimpIA-vertical-color.png" alt="Logo OlimpIA vertical Color"/>
    <div class="logo-label">Versión vertical — Color</div>
  </div>
  <div class="logo-card dark">
    <img src="Logo OlimpIA - Imágenes/Logo-OlimpIA-vertical-blanco.png" alt="Logo OlimpIA vertical Blanco"/>
    <div class="logo-label">Versión vertical — Blanco</div>
  </div>
  <div class="logo-card light">
    <img src="Logo OlimpIA - Imágenes/Símbolo-OlimpIA.png" alt="Símbolo OlimpIA"/>
    <div class="logo-label">Símbolo</div>
  </div>
  <div class="logo-card light">
    <img src="Logo OlimpIA - Imágenes/Nombre-OlimpIA.png" alt="Nombre OlimpIA"/>
    <div class="logo-label">Nombre / Wordmark</div>
  </div>
</div>

<div class="info-box">
  <strong>Versión principal:</strong> Siempre que sea posible se aplicará la marca en su versión horizontal a color.<br>
  <strong>Versión positivo (blanco):</strong> En caso de que el fondo sea oscuro se utilizará la versión en blanco.
</div>

---

### Área de seguridad

<div class="safety-box">
  <p>El <strong>área de seguridad</strong> equivale a una <strong>"O"</strong> del logotipo alrededor del mismo.</p>
  <p>La separación entre el símbolo y la palabra se define con <strong>dos "i" mayúscula</strong>, aplica para ambas versiones (horizontal y vertical).</p>
  <br/>
  <table class="size-table" style="max-width:500px;margin:0 auto;">
    <thead>
      <tr>
        <th>Versión</th>
        <th>Tamaño mínimo digital</th>
        <th>Tamaño mínimo impreso</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Horizontal</td>
        <td>100 px de ancho</td>
        <td>3,5 cm de ancho</td>
      </tr>
      <tr>
        <td>Vertical</td>
        <td>70 px de ancho</td>
        <td>2,5 cm de ancho</td>
      </tr>
    </tbody>
  </table>
</div>

---

### Cobranding

<div class="cobranding-box">
  <h4>📐 Reglas de Cobranding</h4>
  <ul>
    <li>Logotipo de OlimpIA: <strong>133 px de ancho × 29 px de alto</strong> (versión de referencia).</li>
    <li><strong>Línea de separación:</strong> Color <code>#838383</code>, 0,83 px de ancho × 29 px de alto.</li>
    <li>El logo aliado estará a <strong>dos "O"</strong> de distancia del logo de OlimpIA. La línea de separación se ubicará en la mitad de ese espacio.</li>
    <li>El logo de la marca aliada <strong>no debe superar el alto</strong> del logo de OlimpIA.</li>
    <li>Nombre de producto/servicio: Tipografía Poppins Regular, color <code>#182244</code>.</li>
    <li>Si el formato no lo permite, es posible usar la versión vertical.</li>
    <li>Siempre se debe conservar la proporción entre el logo y la línea de separación al escalarlos.</li>
  </ul>
</div>

---

### Aplicaciones incorrectas

<div class="do-dont">
  <div class="do-box">
    <h4>✅ Correcto</h4>
    <ul>
      <li>Usar el logo en sus proporciones originales</li>
      <li>Respetar el área de seguridad alrededor del logo</li>
      <li>Usar la versión blanca sobre fondos oscuros</li>
      <li>Usar la versión color sobre fondos claros</li>
      <li>Garantizar contraste suficiente en todas las aplicaciones</li>
      <li>Mantener la separación correcta en cobranding</li>
    </ul>
  </div>
  <div class="dont-box">
    <h4>❌ Incorrecto</h4>
    <ul>
      <li>Aplicar colores no autorizados al logotipo</li>
      <li>Deformar o escalar desproporcionadamente el logo</li>
      <li>No respetar el área de seguridad</li>
      <li>Usar el logo sobre fondos sin contraste suficiente</li>
      <li>Añadir sombras, efectos o degradados no aprobados</li>
      <li>Rotar o inclinar el logotipo</li>
      <li>Superponer texto sobre el logo</li>
    </ul>
  </div>
</div>

<hr class="divider"/>

<div class="section-header" id="02-tipografía-corporativa">
  <div class="section-number">02</div>
  <div class="section-title">Tipografía Corporativa</div>
</div>

<div class="card">
<h3>Familia Poppins</h3>
<p>La tipografía corporativa seleccionada principal es la perteneciente a la familia <strong>Poppins</strong>.</p>
<p>Poppins es una tipografía <em>geométrica sans-serif</em>, diseñada por <strong>Ninad Kale</strong> y <strong>Jonny Pinhorn</strong> para Indian Type Foundry en 2014. Cuenta con diferentes variantes lo cual la hace una tipografía versátil para su uso.</p>
</div>

<div class="type-alphabet">
ABCDEFGHIJKLMNÑOPQRSTUVWXYZ<br/>
abcdefghijklmnñopqrstuvwxyz<br/>
0 1 2 3 4 5 6 7 8 9
</div>

### Jerarquía tipográfica

<div class="type-showcase">
  <div class="type-card">
    <div class="weight-name">Títulos</div>
    <div class="sample-text" style="font-weight:900;">Poppins<br/>Black</div>
    <div class="size-range">🔡 Tamaño recomendado: <strong>35 px – 45 px</strong></div>
  </div>
  <div class="type-card">
    <div class="weight-name">Subtítulos</div>
    <div class="sample-text" style="font-weight:700;">Poppins<br/>Bold</div>
    <div class="size-range">🔡 Tamaño recomendado: <strong>20 px – 30 px</strong></div>
  </div>
  <div class="type-card">
    <div class="weight-name">Párrafos</div>
    <div class="sample-text" style="font-weight:500;">Poppins<br/>Medium</div>
    <div class="size-range">🔡 Tamaño recomendado: <strong>11 px – 14 px</strong></div>
  </div>
  <div class="type-card">
    <div class="weight-name">Párrafos</div>
    <div class="sample-text" style="font-weight:400;">Poppins<br/>Regular</div>
    <div class="size-range">🔡 Tamaño recomendado: <strong>11 px – 14 px</strong></div>
  </div>
  <div class="type-card">
    <div class="weight-name">Párrafos</div>
    <div class="sample-text" style="font-weight:300;">Poppins<br/>Light</div>
    <div class="size-range">🔡 Tamaño recomendado: <strong>11 px – 14 px</strong></div>
  </div>
</div>

<div class="info-box">
  <strong>Nota:</strong> Los archivos de fuente Poppins están incluidos en la carpeta <code>Tipografía corporativa - Poppins/</code> de este repositorio en formatos TTF.
</div>

<hr class="divider"/>

<div class="section-header" id="03-color">
  <div class="section-number">03</div>
  <div class="section-title">Color</div>
</div>

### Color primario

<div class="color-grid">
  <div class="color-chip">
    <div class="color-swatch" style="background:#0182C4;">
      <span class="hex">#0182C4</span>
    </div>
    <div class="color-info">
      <div class="color-name">Process Blue U</div>
      <div class="color-role">Color primario</div>
      <div class="color-meaning">Confianza, responsabilidad, madurez, creatividad, innovación y diversificación. Es el color del logo y el principal de la marca. Sus variaciones pueden usarse en comunicaciones, pero <strong>jamás</strong> en el logo.</div>
    </div>
  </div>
</div>

### Color complementario

<div class="color-grid">
  <div class="color-chip">
    <div class="color-swatch" style="background:#002F47;">
      <span class="hex">#002F47</span>
    </div>
    <div class="color-info">
      <div class="color-name">Blue Ocean</div>
      <div class="color-role">Color complementario</div>
      <div class="color-meaning">Protección, seriedad</div>
    </div>
  </div>
</div>

### Colores de acento

<div class="color-grid">
  <div class="color-chip">
    <div class="color-swatch" style="background:#00D6F9;">
      <span class="hex">#00D6F9</span>
    </div>
    <div class="color-info">
      <div class="color-name">Azul Innovación</div>
      <div class="color-role">Color acento</div>
      <div class="color-meaning">Tecnología, reflexión</div>
    </div>
  </div>
  <div class="color-chip">
    <div class="color-swatch" style="background:#1389FB;">
      <span class="hex">#1389FB</span>
    </div>
    <div class="color-info">
      <div class="color-name">Azul Seguridad</div>
      <div class="color-role">Color acento</div>
      <div class="color-meaning">Confianza, inteligencia</div>
    </div>
  </div>
  <div class="color-chip">
    <div class="color-swatch" style="background:#7EEC90;">
      <span class="hex" style="color:rgba(0,47,71,0.8);text-shadow:none;">#7EEC90</span>
    </div>
    <div class="color-info">
      <div class="color-name">Verde Solución</div>
      <div class="color-role">Color acento</div>
      <div class="color-meaning">Equilibrio, tranquilidad</div>
    </div>
  </div>
  <div class="color-chip">
    <div class="color-swatch" style="background:#F7EC28;">
      <span class="hex" style="color:rgba(0,47,71,0.8);text-shadow:none;">#F7EC28</span>
    </div>
    <div class="color-info">
      <div class="color-name">Amarillo Creativo</div>
      <div class="color-role">Color acento</div>
      <div class="color-meaning">Originalidad, curiosidad</div>
    </div>
  </div>
  <div class="color-chip">
    <div class="color-swatch" style="background:#5A26EE;">
      <span class="hex">#5A26EE</span>
    </div>
    <div class="color-info">
      <div class="color-name">Morado Tech</div>
      <div class="color-role">Color acento</div>
      <div class="color-meaning">Visión, autenticidad</div>
    </div>
  </div>
  <div class="color-chip">
    <div class="color-swatch" style="background:#F5659A;">
      <span class="hex">#F5659A</span>
    </div>
    <div class="color-info">
      <div class="color-name">Rosa Neuronal</div>
      <div class="color-role">Color acento</div>
      <div class="color-meaning">Armonía, sabiduría</div>
    </div>
  </div>
</div>

### Aplicación en portadas

<div class="card">
<h3>Criterios de uso del color</h3>
<ul>
  <li>En portadas de presentaciones y/o brochures se pueden usar <strong>contrastes entre los colores corporativos</strong>.</li>
  <li>El uso de los colores dependerá de si es información <em>corporativa</em>, de un <em>producto</em> y/o <em>servicio</em>.</li>
  <li>Tratamiento de imagen: <strong>degradados</strong> en la gama de colores azules y morados, con <strong>patrones de textura geométrica</strong> de fondo.</li>
</ul>
</div>

<hr class="divider"/>

<div class="section-header" id="04-iconografía">
  <div class="section-number">04</div>
  <div class="section-title">Iconografía</div>
</div>

<div class="card">
<h3>Criterios de uso de íconos</h3>
<p>Los íconos utilizados en la comunicación de la organización siguen los criterios gráficos previamente establecidos. Se utilizan los <strong>colores de acento</strong> para dar mejor contraste y coherencia visual.</p>
<p>Es importante asegurar la <strong>legibilidad del ícono</strong> en cualquier aplicación, respetando el lineamiento gráfico establecido.</p>
</div>

<div class="info-box">
  <strong>Lineamientos:</strong><br/>
  • Los íconos deben integrarse dentro de la gama de <strong>colores corporativos acento</strong>.<br/>
  • Se deben usar en tamaños que garanticen su legibilidad tanto en medios digitales como impresos.<br/>
  • No se deben combinar estilos de íconos diferentes (p. ej. línea con relleno sólido) en la misma pieza.
</div>

<hr class="divider"/>

<div class="section-header" id="05-fotografía">
  <div class="section-number">05</div>
  <div class="section-title">Fotografía</div>
</div>

<div class="photo-style">
  <h4>📸 Estilo de fotografía</h4>
  <ul>
    <li>Las fotografías deben reflejar <strong>tecnología, cercanía y modernidad</strong>.</li>
    <li>Se aplica un tratamiento de imagen con <strong>degradados en tonos azules y morados</strong>.</li>
    <li>Los patrones llevan una <strong>textura de fondo con figuras geométricas</strong>.</li>
    <li>Las imágenes deben tener <strong>alto contraste</strong> para garantizar la legibilidad de los elementos superpuestos.</li>
    <li>Evitar fotografías de archivo genéricas; preferir imágenes que transmitan <strong>innovación y confianza digital</strong>.</li>
  </ul>
</div>

<hr class="divider"/>

<div class="section-header" id="06-aplicaciones">
  <div class="section-number">06</div>
  <div class="section-title">Aplicaciones</div>
</div>

<div class="card">
<h3>Ejemplos de uso de la marca</h3>
<p>A continuación se muestran algunos contextos donde la marca OlimpIA cobra vida, manteniendo la coherencia visual en todos los puntos de contacto.</p>
</div>

<div class="app-examples">
  <div class="app-example" style="background:linear-gradient(135deg,#002F47,#0182C4);">
    <div class="app-name">Presentaciones</div>
    <div class="app-title">Portadas corporativas con degradados azules y logo en versión blanca</div>
  </div>
  <div class="app-example" style="background:linear-gradient(135deg,#0182C4,#00D6F9);">
    <div class="app-name">Brochures</div>
    <div class="app-title">Colores acento para seccionar información y destacar datos clave</div>
  </div>
  <div class="app-example" style="background:linear-gradient(135deg,#5A26EE,#1389FB);">
    <div class="app-name">Digital / Web</div>
    <div class="app-title">Interfaz con tipografía Poppins, íconos acento y fotografía con tratamiento de color</div>
  </div>
  <div class="app-example" style="background:linear-gradient(135deg,#002F47,#5A26EE);">
    <div class="app-name">Co-branding</div>
    <div class="app-title">Logo OlimpIA + línea separadora + logo aliado respetando proporciones</div>
  </div>
</div>

<div class="info-box">
  <strong>Tagline de marca:</strong> <em>"Soluciones basadas en IA para construir confianza digital"</em>
</div>

---

<div class="footer">
  <strong>OlimpIA</strong> · Manual de Marca · Versión 1.0 · 2024<br/>
  Documento de uso interno y externo. Todos los derechos reservados.<br/>
  <a href="https://github.com/MbarriosOlimpia/2024ManualMarca" style="color:#00D6F9;">github.com/MbarriosOlimpia/2024ManualMarca</a>
</div>
