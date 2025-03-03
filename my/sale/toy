<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Дитяча м’яка іграшка Гусь</title>
  <style>
    /* Підключення шрифту Fredoka з Google Fonts */
    @import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@300;400;500;600&display=swap');
    
    /* Базові стилі та дитяча пастельна кольорова гама */
    body {
      font-family: 'Fredoka', sans-serif;
      background-color: #FFF8F0;
      color: #333;
      margin: 0;
      padding: 0;
      line-height: 1.6;
    }
    .container {
      max-width: 1200px;
      margin: auto;
      padding: 20px;
    }
    header {
      text-align: center;
      padding: 40px 20px;
      background-color: #FFEBE0;
      border-bottom: 2px solid #FDD3B1;
    }
    header h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
      color: #E27D60;
    }
    header p {
      font-size: 1.2em;
      color: #555;
    }
    section {
      padding: 40px 20px;
      margin-bottom: 30px;
    }
    .section-title {
      text-align: center;
      font-size: 2em;
      margin-bottom: 20px;
      color: #E8A87C;
    }
    .description, .specifications, .reviews, .related, .shipping-guarantee, .order {
      background-color: #FFFFFF;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    /* Опис */
    .description p {
      font-size: 1.1em;
      text-align: center;
    }
    /* Характеристики */
    .specifications p {
      font-size: 1.1em;
      margin: 10px 0;
    }
    
    /* --------- Слайдер --------- */
    .slider {
      max-width: 600px;
      margin: 20px auto;
      position: relative;
      overflow: hidden;
      border-radius: 10px;
    }
    .slides img {
      display: none;
      width: 100%;
    }
    
    /* Блок промо (Заощаджуй прямо зараз!) */
    .promo {
      text-align: center;
      margin-bottom: 30px;
    }
    .promo-box {
      display: inline-block;
      background: #005555;
      color: #fff;
      padding: 20px;
      border-radius: 10px;
    }
    .promo-box h2 {
      margin: 0 0 10px 0;
      font-size: 1.5em;
    }
    .promo-box p {
      margin: 5px 0;
      font-size: 1.1em;
    }
    /* Нова секція з кнопкою "Замовити зі знижкою" */
    .order-discount {
      text-align: center;
      margin-bottom: 30px;
    }
    .order-discount button {
      background-color: #E27D60;
      color: #fff;
      padding: 15px 30px;
      font-size: 1.2em;
      border: none;
      cursor: pointer;
      border-radius: 5px;
      transition: background-color 0.3s, transform 0.2s ease-in-out;
    }
    .order-discount button:hover {
      background-color: #C06C50;
      transform: scale(1.05);
    }
    
    /* Відгуки */
    .review-cards {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }
    .review-card {
      background: #fff;
      border: 1px solid #FDD3B1;
      border-radius: 10px;
      width: 250px;
      padding: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .review-card img {
      border-radius: 5px;
      margin-bottom: 10px;
      width: 100%;
    }
    .review-card p {
      margin: 0;
      margin-bottom: 8px;
    }
    .review-card p:last-child {
      margin-bottom: 0;
    }
    .review-card .stars {
      color: #E27D60;
    }
    
    /* Супутні товари */
    .related-products {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-around;
      gap: 20px;
    }
    .related-products .product {
      flex: 1 1 calc(33.333% - 20px);
      max-width: 100%;
      background-color: #FFFAF2;
      padding: 10px;
      border: 1px solid #FDD3B1;
      border-radius: 10px;
      text-align: center;
    }
    .related-products .product img {
      border-radius: 5px;
      margin-bottom: 10px;
    }
    /* Ціни */
    .price-block {
      margin-bottom: 10px;
    }
    .old-price {
      text-decoration: line-through;
      color: #999;
      margin-right: 5px;
    }
    .new-price {
      color: #E27D60;
      font-size: 1.2em;
      font-weight: bold;
    }
    
    /* Блок для перемикача "Ні / Так" */
    .toggle-container {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
      margin-top: 5px;
    }
    .switch {
      position: relative;
      display: inline-block;
      width: 50px;
      height: 24px;
    }
    .switch input {
      opacity: 0;
      width: 0;
      height: 0;
    }
    .slider-switch {
      position: absolute;
      cursor: pointer;
      top: 0; 
      left: 0;
      right: 0;
      bottom: 0;
      background-color: #ccc;
      transition: .4s;
      border-radius: 24px;
    }
    .slider-switch:before {
      position: absolute;
      content: "";
      height: 18px;
      width: 18px;
      left: 3px;
      bottom: 3px;
      background-color: white;
      transition: .4s;
      border-radius: 50%;
    }
    input:checked + .slider-switch {
      background-color: #E27D60;
    }
    input:checked + .slider-switch:before {
      transform: translateX(26px);
    }
    
    /* Стиль для вибору кількості в товарі */
    .product-quantity {
      font-size: 0.8em;
      margin-top: 5px;
    }
    .product-quantity select {
      padding: 5px;
      font-size: 1em;
      border-radius: 3px;
      border: 1px solid #ccc;
    }
    
    /* Форма замовлення */
    .order form {
      max-width: 500px;
      margin: auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }
    .order input, .order button, .order select {
      padding: 10px;
      font-size: 1em;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    .order input, .order select {
      padding: 15px;
      font-size: 1.1em;
    }
    .order input:focus, .order select:focus {
      outline: 2px solid #E27D60;
    }
    .order button {
      background-color: #E27D60;
      color: #fff;
      border: none;
      cursor: pointer;
      transition: background 0.3s, transform 0.2s ease-in-out;
    }
    .order button:hover {
      background-color: #C06C50;
      transform: scale(1.05);
    }
    
    /* Доставка та гарантія */
    .shipping-guarantee {
      margin-top: 30px;
    }
    .shipping-guarantee h2 {
      margin-bottom: 30px;
    }
    .guarantee-wrapper {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 40px;
    }
    .guarantee-item {
      max-width: 200px;
      text-align: center;
    }
    .guarantee-item img {
      width: 64px;
      height: 64px;
      margin-bottom: 15px;
    }
    .guarantee-item h3 {
      font-size: 1.1em;
      color: #333;
      margin-bottom: 10px;
    }
    .guarantee-item p {
      font-size: 0.95em;
      color: #666;
      line-height: 1.4;
    }
    
    /* Футер */
    footer {
      text-align: center;
      padding: 20px;
      background-color: #FFEBE0;
      border-top: 2px solid #FDD3B1;
      font-size: 0.9em;
      color: #777;
    }
    footer p {
      margin: 5px 0;
    }
    footer a {
      color: inherit;
      text-decoration: underline;
      cursor: pointer;
    }
    
    /* Стилі модального вікна */
    .modal {
      display: none; /* приховано за замовчуванням */
      position: fixed;
      z-index: 1000;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      overflow: auto;
      background-color: rgba(0,0,0,0.5);
    }
    .modal-content {
      background-color: #fefefe;
      margin: 10% auto;
      padding: 20px;
      border: 1px solid #888;
      width: 80%;
      max-width: 600px;
      border-radius: 10px;
      position: relative;
    }
    .close {
      color: #aaa;
      position: absolute;
      right: 15px;
      top: 10px;
      font-size: 28px;
      font-weight: bold;
      cursor: pointer;
    }
    .close:hover,
    .close:focus {
      color: black;
      text-decoration: none;
    }
    .modal-text p {
      margin-bottom: 15px;
      line-height: 1.5;
    }
  </style>
</head>
<body>

<div class="container">
  <!-- Заголовок -->
  <header>
    <h1>Дитяча м’яка іграшка Гусь</h1>
    <p>Найкращий друг для вашої дитини — ніжний, затишний та завжди поруч!</p>
  </header>
  
  <!-- Слайдер с фото гуся -->
  <section class="slider">
    <div class="slides">
      <!-- Нові слайди -->
      <img src="https://images.prom.ua/4365671825_w640_h640_4365671825.jpg" alt="Новый слайд 1">
      <img src="https://images.prom.ua/5853357988_w640_h640_5853357988.jpg" alt="Новый слайд 2">
      <img src="https://content.rozetka.com.ua/goods/images/big/357134972.jpg" alt="Новый слайд 3">
    </div>
  </section>
  
  <!-- Блок промо (Заощаджуй прямо зараз!) -->
  <section class="promo">
    <div class="promo-box">
      <h2>ЗАОЩАДЖУЙ ПРЯМО ЗАРАЗ!</h2>
      <p>2 шт = 468 грн ( знижка -30 грн )</p>
      <p>3 шт = 647 грн ( знижка -100 грн )</p>
    </div>
  </section>
  
  <!-- Нова кнопка "Замовити зі знижкою" -->
  <section class="order-discount">
    <button onclick="document.getElementById('order').scrollIntoView({ behavior: 'smooth' });">
      Замовити зі знижкою
    </button>
  </section>
  
  <!-- Опис -->
  <section class="description">
    <h2 class="section-title">Опис</h2>
    <p>Іграшка "Гусь" створена з любов’ю та турботою, щоб дарувати комфорт та радість кожному малюку. Вона допомагає розвивати уяву та створює затишну атмосферу в дитячій кімнаті.</p>
    <p>Ця м’яка іграшка не лише забезпечує тепло та комфорт, але й стимулює творчість та розвиває дрібну моторику. Виготовлена з високоякісних, гіпоалергенних матеріалів, вона стане незамінним другом для будь-якої дитини.</p>
  </section>
  
  <!-- Характеристики -->
  <section class="specifications" style="text-align: center;">
    <h2 class="section-title">Характеристики</h2>
    <p><strong>Розміри:</strong> 50 см, 70 см, 90 см, 110 см, 130 см</p>
    <p><strong>Матеріал:</strong> Гіпоалергенна тканина високої якості</p>
    <p><strong>Колір:</strong> Білий, Жовтий, Рожевий</p>
  </section>
  
  <!-- Відгуки -->
  <section class="reviews" style="text-align:center; padding:20px;">
    <h2 class="section-title">Відгуки покупців</h2>
    <p style="font-size:1.2em; color:#E27D60; font-weight:bold;">
      97,5% покупців відзначили якість товару!
    </p>
    <div class="review-cards">
      <!-- 1 -->
      <div class="review-card">
        <img src="https://via.placeholder.com/220?text=Дитячий+Плед" alt="Відгук Плед">
        <p style="font-weight:bold; margin-bottom:5px;">Тетяна</p>
        <p class="stars">★★★★★</p>
        <p>
          "Замовила дитячий плед разом з гусем. Дуже якісний та м'який! Донька у захваті."
        </p>
      </div>
      <!-- 2 -->
      <div class="review-card">
        <img src="https://via.placeholder.com/220?text=М’яка+Іграшка" alt="Відгук Іграшка">
        <p style="font-weight:bold; margin-bottom:5px;">Роман</p>
        <p class="stars">★★★★★</p>
        <p>
          "Окрім гуса, взяли ще м'яку іграшку. Діти не розлучаються з ними ні на хвилину!"
        </p>
      </div>
      <!-- 3 -->
      <div class="review-card">
        <img src="https://via.placeholder.com/220?text=Плед+і+Гусь" alt="Відгук Плед і Гусь">
        <p style="font-weight:bold; margin-bottom:5px;">Олена</p>
        <p class="stars">★★★★★</p>
        <p>
          "Плед і Гусь — ідеальне поєднання для затишку. Рекомендую всім батькам!"
        </p>
      </div>
      <!-- 4 -->
      <div class="review-card">
        <img src="https://via.placeholder.com/220?text=Іграшковий+телефон" alt="Відгук Іграшковий телефон">
        <p style="font-weight:bold; margin-bottom:5px;">Світлана</p>
        <p class="stars">★★★★☆</p>
        <p>
          "Купили іграшковий телефон у комплекті з гусем. Все супер, дитина дуже задоволена!"
        </p>
      </div>
    </div>
  </section>
  
  <!-- Супутні товари -->
  <section class="related">
    <h2 class="section-title">Разом з цим купують</h2>
    <div class="related-products">
      
      <!-- БЛОК ПОДУШКИ (ИЗМЕНЁН) -->
      <div class="product" style="display: flex; align-items: flex-start; gap: 20px;">
        <!-- Левая часть: изображение -->
        <div style="flex: 0 0 auto;">
          <img
            src="https://le-vele.com.ua/image/cache/webp/data/viluta/7/age-catalog-Podushki-RELAX-20collection-BABY_RELAX_1-800x800.webp"
            alt="Дитяча подушка"
            class="clickable-pillow"
            style="width:150px; cursor:pointer;"
          >
        </div>
        <!-- Правая часть: описание, характеристики и прочее -->
        <div style="flex: 1;">
          <p>Зручна та м'яка подушка для солодкого сну</p>
          <p style="font-size: 0.8em; color: #666; margin: 0 0 10px;">
            <strong>Характеристики:</strong><br>
            • Розмір: 50×70 см<br>
            • Наповнювач: cиліконізоване волокно<br>
            • Чохол: гіпоалергенна мікрофібра
          </p>
          <div class="price-block">
            <span class="old-price">199</span>
            <span class="new-price">80 грн</span>
          </div>
          <p>Додати до замовлення?</p>
          <div class="toggle-container">
            <span>Ні</span>
            <label class="switch">
              <input type="checkbox">
              <span class="slider-switch"></span>
            </label>
            <span>Так</span>
          </div>
          <div class="product-quantity" style="margin-top:10px;">
            <label>Оберіть кількість:</label>
            <select>
              <option value="1" selected>1</option>
              <option value="2">2</option>
              <option value="3">3</option>
              <option value="4">4</option>
              <option value="5">5</option>
              <option value="6">6</option>
              <option value="7">7</option>
              <option value="8">8</option>
              <option value="9">9</option>
              <option value="10">10</option>
            </select>
          </div>
          <div class="product-color" style="margin-top:10px;">
            <span>Оберіть колір:</span>
            <input type="checkbox" name="color1" value="Білий"> <label>Білий</label>
            <input type="checkbox" name="color1" value="Жовтий"> <label>Жовтий</label>
            <input type="checkbox" name="color1" value="Рожевий"> <label>Рожевий</label>
          </div>
        </div>
      </div>
      
      <!-- БЛОК ДИТЯЧИЙ ПЛЕД (ИЗМЕНЁН) -->
      <div class="product" style="display: flex; align-items: flex-start; gap: 20px;">
        <!-- Левая часть: изображение -->
        <div style="flex: 0 0 auto;">
          <img 
            src="https://oba-na.com/image/cache/webp/catalog/demo/11211_1-1000x1000.webp" 
            alt="Дитячий плед" 
            class="clickable-pled"
            style="width:150px; cursor:pointer;"
          >
        </div>
        <!-- Правая часть: описание и краткие характеристики -->
        <div style="flex: 1;">
          <p>Теплий плед для затишку та комфорту</p>
          <p style="font-size: 0.8em; color: #666; margin: 0 0 10px;">
            <strong>Характеристики:</strong><br>
            • Матеріал: 100% м'який фліс<br>
            • Розмір: 100x150 см<br>
            • Догляд: машинне прання
          </p>
          <div class="price-block">
            <span class="old-price">199</span>
            <span class="new-price">80 грн</span>
          </div>
          <p>Додати до замовлення?</p>
          <div class="toggle-container">
            <span>Ні</span>
            <label class="switch">
              <input type="checkbox">
              <span class="slider-switch"></span>
            </label>
            <span>Так</span>
          </div>
          <div class="product-quantity" style="margin-top:10px;">
            <label>Оберіть кількість:</label>
            <select>
              <option value="1" selected>1</option>
              <option value="2">2</option>
              <option value="3">3</option>
              <option value="4">4</option>
              <option value="5">5</option>
              <option value="6">6</option>
              <option value="7">7</option>
              <option value="8">8</option>
              <option value="9">9</option>
              <option value="10">10</option>
            </select>
          </div>
          <div class="product-color" style="margin-top:10px;">
            <span>Оберіть колір:</span>
            <input type="checkbox" name="color2" value="Білий"> <label>Білий</label>
            <input type="checkbox" name="color2" value="Жовтий"> <label>Жовтий</label>
            <input type="checkbox" name="color2" value="Рожевий"> <label>Рожевий</label>
          </div>
        </div>
      </div>
      
      <!-- Остальные блоки товаров остаются без изменений -->
      <!-- 3 -->
      <div class="product">
        <img src="https://via.placeholder.com/150?text=Ковдра" alt="Дитяча ковдра">
        <p>Легка ковдра, що зігріває у прохолодні ночі</p>
        <div class="price-block">
          <span class="old-price">199</span>
          <span class="new-price">80 грн</span>
        </div>
        <p>Додати до замовлення?</p>
        <div class="toggle-container">
          <span>Ні</span>
          <label class="switch">
            <input type="checkbox">
            <span class="slider-switch"></span>
          </label>
          <span>Так</span>
        </div>
        <div class="product-quantity">
          <label>Оберіть кількість:</label>
          <select>
            <option value="1" selected>1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
        </div>
        <div class="product-color">
          <span>Оберіть колір:</span>
          <input type="checkbox" name="color3" value="Білий"> <label>Білий</label>
          <input type="checkbox" name="color3" value="Жовтий"> <label>Жовтий</label>
          <input type="checkbox" name="color3" value="Рожевий"> <label>Рожевий</label>
        </div>
      </div>
      
      <!-- 4 -->
      <div class="product">
        <img src="https://via.placeholder.com/150?text=Іграшковий+телефон" alt="Іграшковий телефон">
        <p>Навчальний телефон для розвитку уяви</p>
        <div class="price-block">
          <span class="old-price">199</span>
          <span class="new-price">80 грн</span>
        </div>
        <p>Додати до замовлення?</p>
        <div class="toggle-container">
          <span>Ні</span>
          <label class="switch">
            <input type="checkbox">
            <span class="slider-switch"></span>
          </label>
          <span>Так</span>
        </div>
        <div class="product-quantity">
          <label>Оберіть кількість:</label>
          <select>
            <option value="1" selected>1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
        </div>
        <div class="product-color">
          <span>Оберіть колір:</span>
          <input type="checkbox" name="color4" value="Білий"> <label>Білий</label>
          <input type="checkbox" name="color4" value="Жовтий"> <label>Жовтий</label>
          <input type="checkbox" name="color4" value="Рожевий"> <label>Рожевий</label>
        </div>
      </div>
      
      <!-- 5 -->
      <div class="product">
        <img src="https://via.placeholder.com/150?text=М’яка+подушка" alt="М’яка подушка">
        <p>Додаткова м’яка подушка з приємною текстурою</p>
        <div class="price-block">
          <span class="old-price">199</span>
          <span class="new-price">80 грн</span>
        </div>
        <p>Додати до замовлення?</p>
        <div class="toggle-container">
          <span>Ні</span>
          <label class="switch">
            <input type="checkbox">
            <span class="slider-switch"></span>
          </label>
          <span>Так</span>
        </div>
        <div class="product-quantity">
          <label>Оберіть кількість:</label>
          <select>
            <option value="1" selected>1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
        </div>
        <div class="product-color">
          <span>Оберіть колір:</span>
          <input type="checkbox" name="color5" value="Білий"> <label>Білий</label>
          <input type="checkbox" name="color5" value="Жовтий"> <label>Жовтий</label>
          <input type="checkbox" name="color5" value="Рожевий"> <label>Рожевий</label>
        </div>
      </div>
      
      <!-- 6 -->
      <div class="product">
        <img src="https://via.placeholder.com/150?text=Кубики" alt="Дитячі кубики">
        <p>Кубики для розвитку дрібної моторики та логіки</p>
        <div class="price-block">
          <span class="old-price">199</span>
          <span class="new-price">80 грн</span>
        </div>
        <p>Додати до замовлення?</p>
        <div class="toggle-container">
          <span>Ні</span>
          <label class="switch">
            <input type="checkbox">
            <span class="slider-switch"></span>
          </label>
          <span>Так</span>
        </div>
        <div class="product-quantity">
          <label>Оберіть кількість:</label>
          <select>
            <option value="1" selected>1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
        </div>
        <div class="product-color">
          <span>Оберіть колір:</span>
          <input type="checkbox" name="color6" value="Білий"> <label>Білий</label>
          <input type="checkbox" name="color6" value="Жовтий"> <label>Жовтий</label>
          <input type="checkbox" name="color6" value="Рожевий"> <label>Рожевий</label>
        </div>
      </div>
      
      <!-- 7 -->
      <div class="product">
        <img src="https://via.placeholder.com/150?text=Розвиваюча+іграшка" alt="Розвиваюча іграшка">
        <p>Захоплива іграшка для навчання та веселощів</p>
        <div class="price-block">
          <span class="old-price">199</span>
          <span class="new-price">80 грн</span>
        </div>
        <p>Додати до замовлення?</p>
        <div class="toggle-container">
          <span>Ні</span>
          <label class="switch">
            <input type="checkbox">
            <span class="slider-switch"></span>
          </label>
          <span>Так</span>
        </div>
        <div class="product-quantity">
          <label>Оберіть кількість:</label>
          <select>
            <option value="1" selected>1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
        </div>
        <div class="product-color">
          <span>Оберіть колір:</span>
          <input type="checkbox" name="color7" value="Білий"> <label>Білий</label>
          <input type="checkbox" name="color7" value="Жовтий"> <label>Жовтий</label>
          <input type="checkbox" name="color7" value="Рожевий"> <label>Рожевий</label>
        </div>
      </div>
      
      <!-- 8 -->
      <div class="product">
        <img src="https://via.placeholder.com/150?text=Мозаїка" alt="Дитяча мозаїка">
        <p>Яскрава мозаїка для творчого мислення</p>
        <div class="price-block">
          <span class="old-price">199</span>
          <span class="new-price">80 грн</span>
        </div>
        <p>Додати до замовлення?</p>
        <div class="toggle-container">
          <span>Ні</span>
          <label class="switch">
            <input type="checkbox">
            <span class="slider-switch"></span>
          </label>
          <span>Так</span>
        </div>
        <div class="product-quantity">
          <label>Оберіть кількість:</label>
          <select>
            <option value="1" selected>1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
        </div>
        <div class="product-color">
          <span>Оберіть колір:</span>
          <input type="checkbox" name="color8" value="Білий"> <label>Білий</label>
          <input type="checkbox" name="color8" value="Жовтий"> <label>Жовтий</label>
          <input type="checkbox" name="color8" value="Рожевий"> <label>Рожевий</label>
        </div>
      </div>
      
      <!-- 9 -->
      <div class="product">
        <img src="https://via.placeholder.com/150?text=Конструктор" alt="Дитячий конструктор">
        <p>Будівельний набір для креативних ідей</p>
        <div class="price-block">
          <span class="old-price">199</span>
          <span class="new-price">80 грн</span>
        </div>
        <p>Додати до замовлення?</p>
        <div class="toggle-container">
          <span>Ні</span>
          <label class="switch">
            <input type="checkbox">
            <span class="slider-switch"></span>
          </label>
          <span>Так</span>
        </div>
        <div class="product-quantity">
          <label>Оберіть кількість:</label>
          <select>
            <option value="1" selected>1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
        </div>
        <div class="product-color">
          <span>Оберіть колір:</span>
          <input type="checkbox" name="color9" value="Білий"> <label>Білий</label>
          <input type="checkbox" name="color9" value="Жовтий"> <label>Жовтий</label>
          <input type="checkbox" name="color9" value="Рожевий"> <label>Рожевий</label>
        </div>
      </div>
      
      <!-- 10 -->
      <div class="product">
        <img src="https://via.placeholder.com/150?text=Настільна+гра" alt="Настільна гра">
        <p>Весела гра для всієї родини</p>
        <div class="price-block">
          <span class="old-price">199</span>
          <span class="new-price">80 грн</span>
        </div>
        <p>Додати до замовлення?</p>
        <div class="toggle-container">
          <span>Ні</span>
          <label class="switch">
            <input type="checkbox">
            <span class="slider-switch"></span>
          </label>
          <span>Так</span>
        </div>
        <div class="product-quantity">
          <label>Оберіть кількість:</label>
          <select>
            <option value="1" selected>1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
        </div>
        <div class="product-color">
          <span>Оберіть колір:</span>
          <input type="checkbox" name="color10" value="Білий"> <label>Білий</label>
          <input type="checkbox" name="color10" value="Жовтий"> <label>Жовтий</label>
          <input type="checkbox" name="color10" value="Рожевий"> <label>Рожевий</label>
        </div>
      </div>
    </div>
  </section>
  
  <!-- Новий блок "Доставка та гарантія" -->
  <section class="shipping-guarantee">
    <h2 class="section-title">Доставка та гарантія</h2>
    <div class="guarantee-wrapper">
      <div class="guarantee-item">
        <img src="https://via.placeholder.com/64?text=Icon" alt="Доставка">
        <h3>Доставка</h3>
        <p>Доставка Новою та Укр поштою протягом 1-3 робочих днів.</p>
      </div>
      <div class="guarantee-item">
        <img src="https://via.placeholder.com/64?text=Icon" alt="Жодних передоплат">
        <h3>Жодних передоплат!</h3>
        <p>Оплата замовлення здійснюється при отриманні товару на пошті.</p>
      </div>
      <div class="guarantee-item">
        <img src="https://via.placeholder.com/64?text=Icon" alt="Гарантія">
        <h3>Гарантія</h3>
        <p>Перед відправкою всі товари проходять ретельну перевірку щодо браку.</p>
      </div>
    </div>
  </section>
  
  <!-- Форма замовлення (контактні дані) -->
  <section class="order" id="order">
    <h2 class="section-title">Замовлення</h2>
    <form id="order-form">
      <label for="name">Ім'я:</label>
      <input type="text" id="name" name="name" placeholder="Ваше ім'я" required>
      
      <label for="phone">Номер телефону:</label>
      <input type="tel" id="phone" name="phone" placeholder="+380 (__) ___-__-__" pattern="^\+380\d{9}$" required>
      
      <!-- Новий ряд: Оберіть кількість і Оберіть розмір -->
      <div style="display: flex; gap: 20px; align-items: flex-end; font-size: 0.9em; margin-top:10px;">
        <div>
          <label for="quantity" style="display: block; font-size: 0.9em;">Оберіть кількість:</label>
          <select id="quantity" name="quantity" required>
            <option value="1" selected>1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
            <option value="5">5</option>
            <option value="6">6</option>
            <option value="7">7</option>
            <option value="8">8</option>
            <option value="9">9</option>
            <option value="10">10</option>
          </select>
        </div>
        <div>
          <label for="size" style="display: block; font-size: 0.9em;">Оберіть розмір:</label>
          <select id="size" name="size" required>
            <option value="50">50 см</option>
            <option value="70">70 см</option>
            <option value="90">90 см</option>
            <option value="110">110 см</option>
            <option value="130">130 см</option>
          </select>
        </div>
      </div>
      
      <!-- Новий ряд для вибору кольору -->
      <div style="font-size:0.8em; margin-top:5px;">
         <span>Оберіть колір:</span>
         <input type="checkbox" name="orderColor" value="Білий"> <label style="font-size:0.8em;">Білий</label>
         <input type="checkbox" name="orderColor" value="Сірий"> <label style="font-size:0.8em;">Сірий</label>
         <input type="checkbox" name="orderColor" value="Бежевий"> <label style="font-size:0.8em;">Бежевий</label>
      </div>
      
      <button type="submit">Надіслати замовлення</button>
    </form>
  </section>
</div>

<!-- Футер -->
<footer>
  <p>2017-2025. Усі права захищені.</p>
  <p><a href="#" id="privacyPolicyLink">Політика конфіденційності</a>.</p>
</footer>

<!-- Модальне вікно для збільшення зображення подушки -->
<div id="pillowModal" class="modal">
  <div class="modal-content" style="max-width:90%; max-height:90%;">
    <span class="close" id="pillowModalClose">&times;</span>
    <img src="https://le-vele.com.ua/image/cache/webp/data/viluta/7/age-catalog-Podushki-RELAX-20collection-BABY_RELAX_1-800x800.webp" alt="Дитяча подушка" style="width:100%;">
  </div>
</div>

<!-- Модальне вікно для збільшення зображення пледа -->
<div id="pledModal" class="modal">
  <div class="modal-content" style="max-width:90%; max-height:90%;">
    <span class="close" id="pledModalClose">&times;</span>
    <img src="https://oba-na.com/image/cache/webp/catalog/demo/11211_1-1000x1000.webp" alt="Дитячий плед" style="width:100%;">
  </div>
</div>

<!-- Скрипти -->
<script>
  document.addEventListener("DOMContentLoaded", function() {
    let slideIndex = 0;
    const slides = document.querySelectorAll(".slides img");
    
    function showSlides() {
      slides.forEach((slide, index) => {
        slide.style.display = (index === slideIndex) ? "block" : "none";
      });
      slideIndex = (slideIndex + 1) % slides.length;
      setTimeout(showSlides, 3000);
    }
    
    showSlides();
  });
</script>

<script>
  document.getElementById("order-form").addEventListener("submit", function(event) {
    let phone = document.getElementById("phone").value;
    if (!phone.match(/^\+380\d{9}$/)) {
      alert("Будь ласка, введіть коректний номер телефону у форматі +380XXXXXXXXX");
      event.preventDefault();
    }
  });
</script>

<script>
  // Скрипт для модального вікна політики конфіденційності
  var modal = document.getElementById("privacyModal");
  var link = document.getElementById("privacyPolicyLink");
  var closeBtn = document.getElementsByClassName("close")[0];

  link.onclick = function(e) {
    e.preventDefault();
    modal.style.display = "block";
  }

  closeBtn.onclick = function() {
    modal.style.display = "none";
  }

  window.onclick = function(event) {
    if (event.target == modal) {
      modal.style.display = "none";
    }
  }
</script>

<script>
  // Скрипт для модального вікна збільшення зображення подушки
  var pillowModal = document.getElementById("pillowModal");
  var pillowImg = document.querySelector(".clickable-pillow");
  var pillowModalClose = document.getElementById("pillowModalClose");

  pillowImg.onclick = function() {
      pillowModal.style.display = "block";
  }

  pillowModalClose.onclick = function() {
      pillowModal.style.display = "none";
  }

  window.addEventListener("click", function(event) {
    if (event.target == pillowModal) {
      pillowModal.style.display = "none";
    }
  });
</script>

<script>
  // Скрипт для модального вікна збільшення зображення пледа
  var pledModal = document.getElementById("pledModal");
  var pledImg = document.querySelector(".clickable-pled");
  var pledModalClose = document.getElementById("pledModalClose");

  pledImg.onclick = function() {
      pledModal.style.display = "block";
  }

  pledModalClose.onclick = function() {
      pledModal.style.display = "none";
  }

  window.addEventListener("click", function(event) {
    if (event.target == pledModal) {
      pledModal.style.display = "none";
    }
  });
</script>

</body>
</html>
