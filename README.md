# Muack
<!doctype html>
<html lang="es">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>TE QUIERO</title>

    <!-- Tipografías -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&family=Merriweather:wght@300;400;700&display=swap" rel="stylesheet" />

    <style>
      :root {
        --bg: #ffe4ec; /* rosa claro */
        --fg: #3d003d;
        --accent: #ff4f9a; /* rosa del corazón */
        --heart: clamp(200px, 45vw, 420px); /* tamaño responsivo del corazón */
      }

      * { box-sizing: border-box; }
      html, body { height: 100%; }
      body {
        margin: 0;
        font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji", "Segoe UI Emoji";
        background: var(--bg);
        color: var(--fg);
        line-height: 1.6;
        padding: 20px;
      }

      header {
        padding: 32px 20px 0;
        text-align: center;
      }

      h1 {
        font-family: Merriweather, Georgia, "Times New Roman", Times, serif;
        font-weight: 700;
        font-size: clamp(2rem, 3vw + 1rem, 3rem);
        margin: 0 0 20px;
        letter-spacing: 0.3px;
        color: var(--accent);
      }

      .poem {
        font-family: Merriweather, Georgia, "Times New Roman", Times, serif;
        font-size: clamp(1.05rem, 1.2vw + 0.9rem, 1.4rem);
        letter-spacing: 0.2px;
        white-space: pre-wrap;
        max-width: 800px;
        margin: 0 auto;
      }

      .stanza { margin: 0 0 1.2em; }

      /* Corazón gigante */
      .heart { display: grid; place-items: center; margin: 60px 0 90px; }

      .heart-wrap { position: relative; width: var(--heart); height: var(--heart); }

      .heart-shape {
        position: absolute;
        inset: 0;
        width: var(--heart);
        height: var(--heart);
        background-color: var(--accent);
        transform: rotate(-45deg);
        border-radius: 14px;
        z-index: 1;
      }
      .heart-shape::before,
      .heart-shape::after {
        content: "";
        position: absolute;
        width: var(--heart);
        height: var(--heart);
        background-color: var(--accent);
        border-radius: 50%;
        z-index: 1;
      }
      .heart-shape::before { top: calc(-0.5 * var(--heart)); left: 0; }
      .heart-shape::after { left: calc(0.5 * var(--heart)); top: 0; }

      .heart-text {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        font-family: Merriweather, Georgia, serif;
        font-weight: 800;
        font-size: clamp(1.6rem, calc(var(--heart) / 5), 4.5rem);
        color: #fff;
        letter-spacing: 0.08em;
        z-index: 2;
        text-align: center;
      }
    </style>
  </head>
  <body>
    <header>
      <h1>TE QUIERO</h1>
    </header>

    <main>
      <div id="poem-text" class="poem" lang="es" aria-label="Texto del poema">
        <p class="stanza">
          Tú, que con tu voz me cautivas<br />
          y con tu risa me llenas de alegría,<br />
          te has convertido en mi aire,<br />
          mi fuente de vida.
        </p>
        <p class="stanza">
          No sé cómo se pueden sentir<br />
          tantas cosas en tan poco tiempo,<br />
          pero soy consciente de lo que siento<br />
          y por qué, mi gustar hacia ti<br />
          es causado por la forma tan hermosa<br />
          en la que me haces sentir<br />
          y el café de tus hermosos ojos<br />
          que me cautivan cuál miel a oso.
        </p>
        <p class="stanza">
          Te pienso, en cada momento y lugar,<br />
          estás en mi mente, en mi vida.<br />
          Un rayo que iluminó mi noche tormentosa,<br />
          alguien que agradezco haber conocido<br />
          y espero no perder.
        </p>
        <p class="stanza">
          Mi niña linda, ganar tu amor<br />
          se ha convertido en mi mayor ambición,<br />
          estoy seguro de que tu ser<br />
          será mi complemento,<br />
          tus labios mi perdición<br />
          y tu voz, la eterna y mejor canción.
        </p>
      </div>

      <div class="heart" aria-label="Corazón con iniciales">
        <div class="heart-wrap">
          <div class="heart-shape"></div>
          <div class="heart-text">E y S</div>
        </div>
      </div>
    </main>
  </body>
</html>
