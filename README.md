<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Our Homemade Liquors</title>
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
    .lang-selector {
      text-align: center;
      margin-bottom: 2rem;
    }
    select {
      font-size: 1rem;
      padding: 0.5rem;
    }
  </style>
</head>
<body>

  <div class="lang-selector">
    <label for="language">🌍 Language:</label>
    <select id="language" onchange="setLanguage(this.value)">
      <option value="en" selected>English</option>
      <option value="it">Italiano</option>
      <option value="es">Español</option>
      <option value="fr">Français</option>
      <option value="de">Deutsch</option>
      <option value="ru">Русский</option>
    </select>
  </div>

  <h1 id="title">Our Homemade Liquors</h1>
  
<p style="text-align:center; margin-top: 0.5rem;">
  <a href="https://revolut.me/michelk36" target="_blank" style="color: #0066cc; font-weight: bold; text-decoration: none;">
    💙 Click here to make a donation if you enjoyed our liqueurs 💙
  </a>
</p>
  <div class="liquore">
    <h2 id="name1">Limoncello</h2>
    <p id="desc1">Ingredients: lemon peels (25% infusion), water, sugar, alcohol</p>
    <p class="percentuale" id="alc1">Alcohol content: 31%</p>
  </div>

  <div class="liquore">
    <h2 id="name2">Herbal Digestif</h2>
    <p id="desc2">Ingredients: wild fennel, mint, laurel, rosemary, basil, cloves, lemon leaves, lemon and orange peels, water, sugar, alcohol</p>
    <p class="percentuale" id="alc2">Alcohol content: 34%</p>
  </div>

  <div class="liquore">
    <h2 id="name3">Rhubarb Liqueur</h2>
    <p id="desc3">Ingredients: rhubarb, water, sugar, alcohol</p>
    <p class="percentuale" id="alc3">Alcohol content: 33%</p>
  </div>

  <div class="liquore">
    <h2 id="name4">Strawberry Liqueur</h2>
    <p id="desc4">Ingredients: water, sugar, local strawberries, alcohol</p>
    <p class="percentuale" id="alc4">Alcohol content: 28%</p>
  </div>

  <div class="liquore">
    <h2 id="name5">Chocolate Liqueur</h2>
    <p id="desc5">Ingredients: milk, heavy cream, dark chocolate, sugar, alcohol</p>
    <p class="percentuale" id="alc5">Alcohol content: 20%</p>
  </div>

  <script>
    const translations = {
      en: {
        title: "Our Homemade Liquors",
        name1: "Limoncello",
        desc1: "Ingredients: lemon peels (25% infusion), water, sugar, alcohol",
        alc1: "Alcohol content: 31%",
        name2: "Herbal Digestif",
        desc2: "Ingredients: wild fennel, mint, laurel, rosemary, basil, cloves, lemon leaves, lemon and orange peels, water, sugar, alcohol",
        alc2: "Alcohol content: 34%",
        name3: "Rhubarb Liqueur",
        desc3: "Ingredients: rhubarb, water, sugar, alcohol",
        alc3: "Alcohol content: 33%",
        name4: "Strawberry Liqueur",
        desc4: "Ingredients: water, sugar, local strawberries, alcohol",
        alc4: "Alcohol content: 28%",
        name5: "Chocolate Liqueur",
        desc5: "Ingredients: milk, heavy cream, dark chocolate, sugar, alcohol",
        alc5: "Alcohol content: 20%"
      },
      it: {
        title: "I Nostri Liquori Artigianali",
        name1: "Limoncello",
        desc1: "Ingredienti: scorze di limoni (infusione al 25%), acqua, zucchero, alcool",
        alc1: "Gradazione alcolica: 31%",
        name2: "Digestivo alle Erbe",
        desc2: "Ingredienti: finocchietto selvatico, menta, alloro, rosmarino, basilico, chiodi di garofano, foglie di limone, scorze di limone e arancia, acqua, zucchero, alcool",
        alc2: "Gradazione alcolica: 34%",
        name3: "Liquore al Rabarbaro",
        desc3: "Ingredienti: rabarbaro, acqua, zucchero, alcool",
        alc3: "Gradazione alcolica: 33%",
        name4: "Liquore alla Fragola",
        desc4: "Ingredienti: acqua, zucchero, fragole locali, alcool",
        alc4: "Gradazione alcolica: 28%",
        name5: "Liquore al Cioccolato",
        desc5: "Ingredienti: latte, panna, cioccolato fondente, zucchero, alcool",
        alc5: "Gradazione alcolica: 20%"
      },
      es: {
        title: "Nuestros Licores Caseros",
        name1: "Limoncello",
        desc1: "Ingredientes: cáscaras de limón (infusión al 25%), agua, azúcar, alcohol",
        alc1: "Contenido alcohólico: 31%",
        name2: "Digestivo de Hierbas",
        desc2: "Ingredientes: hinojo silvestre, menta, laurel, romero, albahaca, clavos, hojas de limón, cáscaras de limón y naranja, agua, azúcar, alcohol",
        alc2: "Contenido alcohólico: 34%",
        name3: "Licor de Ruibarbo",
        desc3: "Ingredientes: ruibarbo, agua, azúcar, alcohol",
        alc3: "Contenido alcohólico: 33%",
        name4: "Licor de Fresa",
        desc4: "Ingredientes: agua, azúcar, fresas locales, alcohol",
        alc4: "Contenido alcohólico: 28%",
        name5: "Licor de Chocolate",
        desc5: "Ingredientes: leche, nata, chocolate negro, azúcar, alcohol",
        alc5: "Contenido alcohólico: 20%"
      },
      fr: {
        title: "Nos Liqueurs Maison",
        name1: "Limoncello",
        desc1: "Ingrédients : zestes de citron (infusion à 25%), eau, sucre, alcool",
        alc1: "Teneur en alcool : 31%",
        name2: "Digestif aux Herbes",
        desc2: "Ingrédients : fenouil sauvage, menthe, laurier, romarin, basilic, clous de girofle, feuilles de citron, zestes de citron et d'orange, eau, sucre, alcool",
        alc2: "Teneur en alcool : 34%",
        name3: "Liqueur de Rhubarbe",
        desc3: "Ingrédients : rhubarbe, eau, sucre, alcool",
        alc3: "Teneur en alcool : 33%",
        name4: "Liqueur à la Fraise",
        desc4: "Ingrédients : eau, sucre, fraises locales, alcool",
        alc4: "Teneur en alcool : 28%",
        name5: "Liqueur au Chocolat",
        desc5: "Ingrédients : lait, crème épaisse, chocolat noir, sucre, alcool",
        alc5: "Teneur en alcool : 20%"
      },
      de: {
        title: "Unsere Hausgemachten Liköre",
        name1: "Limoncello",
        desc1: "Zutaten: Zitronenschalen (25 % Infusion), Wasser, Zucker, Alkohol",
        alc1: "Alkoholgehalt: 31%",
        name2: "Kräuter-Digestif",
        desc2: "Zutaten: wilder Fenchel, Minze, Lorbeer, Rosmarin, Basilikum, Nelken, Zitronenblätter, Zitronen- und Orangenschalen, Wasser, Zucker, Alkohol",
        alc2: "Alkoholgehalt: 34%",
        name3: "Rhabarberlikör",
        desc3: "Zutaten: Rhabarber, Wasser, Zucker, Alkohol",
        alc3: "Alkoholgehalt: 33%",
        name4: "Erdbeerlikör",
        desc4: "Zutaten: Wasser, Zucker, lokale Erdbeeren, Alkohol",
        alc4: "Alkoholgehalt: 28%",
        name5: "Schokoladenlikör",
        desc5: "Zutaten: Milch, Sahne, Zartbitterschokolade, Zucker, Alkohol",
        alc5: "Alkoholgehalt: 20%"
      },
      ru: {
        title: "Наши Домашние Ликеры",
        name1: "Лимончелло",
        desc1: "Ингредиенты: лимонная цедра (настаивание 25%), вода, сахар, спирт",
        alc1: "Крепость: 31%",
        name2: "Травяной Дижестив",
        desc2: "Ингредиенты: дикий фенхель, мята, лавр, розмарин, базилик, гвоздика, лимонные листья, цедра лимона и апельсина, вода, сахар, спирт",
        alc2: "Крепость: 34%",
        name3: "Ликёр из Ревеня",
        desc3: "Ингредиенты: ревень, вода, сахар, спирт",
        alc3: "Крепость: 33%",
        name4: "Клубничный Ликёр",
        desc4: "Ингредиенты: вода, сахар, местная клубника, спирт",
        alc4: "Крепость: 28%",
        name5: "Шоколадный Ликёр",
        desc5: "Ингредиенты: молоко, густые сливки, темный шоколад, сахар, спирт",
        alc5: "Крепость: 20%"
      }
    };

    function setLanguage(lang) {
      const t = translations[lang];
      document.getElementById("title").innerText = t.title;
      for (let i = 1; i <= 5; i++) { // Changed loop limit to 5 to include the new liqueur
        document.getElementById("name" + i).innerText = t["name" + i];
        document.getElementById("desc" + i).innerText = t["desc" + i];
        document.getElementById("alc" + i).innerText = t["alc" + i];
      }
    }

    // Set initial language on page load
    document.addEventListener('DOMContentLoaded', () => {
      setLanguage(document.getElementById('language').value);
    });
  </script>

</body>
</html>
