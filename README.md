# Malta-Liquors
# I Nostri Liquori
<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>I Nostri Liquori</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f9f9f9;
      margin: 0;
      padding: 2rem;
      color: #333;
    }
    h1 {
      text-align: center;
      color: #444;
    }
    .liquore {
      background: white;
      border-radius: 12px;
      padding: 1.5rem;
      margin: 1rem auto;
      max-width: 600px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .liquore h2 {
      margin-top: 0;
      color: #222;
    }
    .percentuale {
      font-weight: bold;
      color: #666;
    }
    footer {
      text-align: center;
      margin-top: 2rem;
      font-size: 0.9em;
      color: #555;
    }
    #languageSelect {
      margin-top: 10px;
    }
    #qrCode {
      display: block;
      margin: 2rem auto;
    }
  </style>
</head>
<body>

  <!-- Titolo -->
  <h1 id="title">I Nostri Liquori Artigianali</h1>

  <!-- Sezioni liquori -->
  <div class="liquore" data-translation-key="liquor1">
    <h2 id="liquor1-title">Limoncello</h2>
    <p id="liquor1-ingredients">Ingredienti: scorze di limoni (infusione al 25%), acqua, zucchero, alcool</p>
    <p class="percentuale" id="liquor1-alcohol">Gradazione alcolica: 31%</p>
  </div>

  <div class="liquore" data-translation-key="liquor2">
    <h2 id="liquor2-title">Digestivo alle Erbe</h2>
    <p id="liquor2-ingredients">Ingredienti: finocchietto selvatico, menta, alloro, rosmarino, basilico, chiodi di garofano, foglie di limone, scorze di limone e arancia, acqua, zucchero, alcool</p>
    <p class="percentuale" id="liquor2-alcohol">Gradazione alcolica: 34%</p>
  </div>

  <div class="liquore" data-translation-key="liquor3">
    <h2 id="liquor3-title">Liquore al Rabarbaro</h2>
    <p id="liquor3-ingredients">Ingredienti: rabarbaro, acqua, zucchero, alcool</p>
    <p class="percentuale" id="liquor3-alcohol">Gradazione alcolica: 33%</p>
  </div>

  <div class="liquore" data-translation-key="liquor4">
    <h2 id="liquor4-title">Liquore alla Fragola</h2>
    <p id="liquor4-ingredients">Ingredienti: acqua, zucchero, fragole locali, alcool</p>
    <p class="percentuale" id="liquor4-alcohol">Gradazione alcolica: 28%</p>
  </div>

  <!-- Sezione footer: ingredienti locali e di stagione -->
  <footer id="footer-text">
    Tutti i liquori sono fatti con ingredienti locali e di stagione (quando disponibili).
  </footer>

  <!-- Selettore lingue -->
  <div style="text-align:center; margin-top:20px;">
    <select id="languageSelect">
      <option value="it">Italiano</option>
      <option value="en">English</option>
    </select>
  </div>

</body>
</html>
