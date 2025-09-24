Tehtävä: Sass → CSS käännös ja sivun tyylitys
Tässä tehtävässä luot valmiille HTML-sivulle muotoilut Sassilla (.scss). Käännät koodin CSS:ksi ja katsot selaimessa, miten ulkoasu muuttuu.
1) Tiedostorakenne
Luo projektillesi seuraava hakemistorakenne:
project/
├─ index.html
├─ scss/
│  ├─ _variables.scss
│  ├─ _mixins.scss
│  ├─ _layout.scss
│  └─ style.scss
└─ css/
   └─ style.css
2) Valmis HTML
Tallenna seuraava sisältö tiedostoon index.html (älä muokkaa sisältöä):
<!doctype html>
<html lang="fi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Sass-harjoitus: Bistro Aurora</title>
  <link rel="stylesheet" href="css/style.css" />
</head>
<body>
  <header class="site-header">
    <div class="container">
      <h1 class="logo">Bistro <span>Aurora</span></h1>
      <nav class="main-nav">
        <a href="#" class="nav-link is-active">Etusivu</a>
        <a href="#" class="nav-link">Menu</a>
        <a href="#" class="nav-link">Varaa</a>
        <a href="#" class="nav-link">Yhteys</a>
      </nav>
      <button class="btn btn-primary">Varaa pöytä</button>
    </div>
  </header>

  <section class="hero">
    <div class="container">
      <h2>Kaupungin rennoin illallispaikka</h2>
      <p>Tuoretta, paikallista ja sesongin mukaan — tervetuloa nauttimaan!</p>
      <a href="#" class="btn btn-secondary">Tutustu menuun</a>
    </div>
  </section>

  <main class="container grid">
    <article class="card">
      <h3>Päivän annos</h3>
      <p>Paistettua siikaa, sitruunarisottoa ja yrttikastiketta.</p>
      <a href="#" class="link">Lue lisää</a>
    </article>

    <article class="card">
      <h3>Kasvisvaihtoehto</h3>
      <p>Paahdettu kukkakaali, mantelia ja chimichurria.</p>
      <a href="#" class="link">Lue lisää</a>
    </article>

    <aside class="sidebar">
      <h4>Aukioloajat</h4>
      <ul class="hours">
        <li>Ma–To 11–22</li>
        <li>Pe 11–00</li>
        <li>La 12–00</li>
        <li>Su 12–21</li>
      </ul>
    </aside>
  </main>

  <footer class="site-footer">
    <div class="container">
      <p>© 2025 Bistro Aurora • Satamakatu 7, 80100 Joensuu</p>
      <nav class="social">
        <a href="#" aria-label="Instagram">@bistroaurora</a>
        <a href="#" aria-label="Facebook">Facebook</a>
      </nav>
    </div>
  </footer>
</body>
</html>
3) Mitä Sassilla pitää toteuttaa
Tee tyylit .scss-tiedostoihin käyttäen seuraavia ominaisuuksia:
1) Muuttujat: värit, typografia ja mitat (variables.scss)
2) Mixin + include: esim. nappi, container, media-kyselyt (mixins.scss)
3) Sisäkkäiset valitsijat ja &-parent (layout.scss)
4) Osittaiset tiedostot ja import pääsisäänmenoon (style.scss)
5) Funktiot ja operaattorit (esim. darken, lighten)
6) Responsiivisuus (grid, sidebar, media query mixin)
7) Komponentit (btn, hero, card jne.)
4) Kääntäminen VS Codessa
Vaihtoehto A: Live Sass Compiler
 - Asenna laajennus Live Sass Compiler
 - Avaa projekti ja paina 'Watch Sass'
 - style.scss käännetään css/style.css-tiedostoksi
Vaihtoehto B: npm sass
 - Suorita projektissa: npm install sass --save-dev
 - Käännä: npx sass scss/style.scss css/style.css --watch
5) Palautus
Palauta projektikansio (HTML + SCSS + käännetty CSS). Lisää kuvakaappaus sivusta sekä lyhyt kuvaus: Mitä Sass-ominaisuuksia käytit ja missä?
