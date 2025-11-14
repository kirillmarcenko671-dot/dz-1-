<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sweet Art - Вкусные моменты вашей жизни</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Sweet Art</h1>
        <p>Вкусные моменты вашей жизни</p>
        <nav>
            <ul>
                <li><a href="#about">О нас</a></li>
                <li><a href="#products">Наши торты</a></li>
                <li><a href="#reviews">Отзывы</a></li>
                <li><a href="#order">Как заказать</a></li>
                <li><a href="#contacts">Контакты</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="about">
            <h2>О нашем уютном деле</h2>
            <p>Мы - команда <strong>Sweet Art</strong>, влюбленная в кондитерское искусство. Каждый наш торт - это уникальная история, созданная с душой и вниманием к деталям.</p>
            <p>Используем только <em>натуральные ингредиенты</em>:
                <ul>
                    <li>Свежие фермерские продукты</li>
                    <li>Натуральные сливки и масло</li>
                    <li>Домашние варенья</li>
                    <li>Ягоды и фрукты по сезону</li>
                </ul>
            </p>
        </section>

        <section id="products">
            <h2>Наши торты</h2>
            
            <article>
                <h3>Торт "Классический Медовик"</h3>
                <p>Нежные медовые коржи с пропитанные сметанным кремом. Классика, которая никогда не подводит.</p>
                <p><strong>Цена:</strong> 2000 руб./кг</p>
            </article>

            <article>
                <h3>Торт "Шоколадная эйфория"</h3>
                <p>Для настоящих любителей шоколада. Бисквит с какао, шоколадный ганаш и сливочный крем.</p>
                <p><strong>Цена:</strong> 2200 руб./кг</p>
            </article>

            <article>
                <h3>Торт "Ягодное наслаждение"</h3>
                <p>Легкий бисквит, свежие сезонные ягоды и воздушный крем. Идеально для летнего праздника.</p>
                <p><strong>Цена:</strong> 2400 руб./кг</p>
            </article>
        </section>

        <section id="reviews">
            <h2>Что говорят наши клиенты</h2>
            
            <blockquote>
                <p>"Заказывала торт на юбилей родителей. Не только красиво, но и невероятно вкусно! Гости были в восторге."</p>
                <cite>Артем, 35 лет</cite>
            </blockquote>

            <blockquote>
                <p>"Каждый год заказываем у вас торт на день рождения ребенка. Дети обожают ваши сладости!"</p>
                <cite>Семья Ивановых</cite>
            </blockquote>
        </section>

        <section id="order">
            <h2>Как сделать заказ</h2>
            <ol>
                <li>Выберите торт или опишите ваши пожелания</li>
                <li>Свяжитесь с нами по телефону или через форму на сайте</li>
                <li>Обсудите детали заказа и дату приготовления</li>
                <li>Получите ваш идеальный торт в назначенный день!</li>
            </ol>
        </section>

        <section id="contacts">
            <h2>Наши контакты</h2>
            <address>
                <p>г. Ростов, ул. Садовая, д. 53</p>
                <p>Телефон: <a href="tel:+79045040016">+7 (999) 123-45-67</a></p>
                <p>Email: <a href="Kitivin@bk.ru">order@sweetart.ru</a></p>
                <p>Время работы: ежедневно с 9:00 до 21:00</p>
            </address>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 Sweet Art. Все права защищены.</p>
        <p>Следите за нами в соцсетях: 
            <a href="#">Instagram</a> | 
            <a href="#">VK</a>
        </p>
    </footer>
</body>
</html>




STYLE.scss


$primary-color: #d46a6a;
$secondary-color: #b85c5c;
$light-color: #f8e3e3;
$accent-color: #f5d0d0;
$text-color: #5a3e36;
$light-text: #8c5e5e;
$background: #fff9f5;
$white: #fff;


@mixin grid($columns, $gap: 2rem) {
  display: grid;
  grid-template-columns: $columns;
  gap: $gap;
}

@mixin flex-center {
  display: flex;
  justify-content: center;
  align-items: center;
}

@mixin card-shadow {
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
}

@mixin hover-effect {
  transition: all 0.3s ease;
  
  &:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
  }
}


* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
  background-color: $background;
  color: $text-color;
  line-height: 1.6;
}


.main-grid {
  display: grid;
  grid-template-rows: auto;
  gap: 4rem;
}


header {
  background: linear-gradient(135deg, $light-color 0%, $accent-color 100%);
  padding: 2rem 1rem;
  text-align: center;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  position: sticky;
  top: 0;
  z-index: 100;
  
  h1 {
    font-size: 3rem;
    color: $primary-color;
    margin-bottom: 0.5rem;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  p {
    font-size: 1.2rem;
    color: $light-text;
    margin-bottom: 1.5rem;
    font-style: italic;
  }
}


nav ul {
  @include grid(repeat(auto-fit, minmax(150px, 1fr)), 1rem);
  list-style: none;
  
  @media (max-width: 768px) {
    grid-template-columns: 1fr;
    gap: 0.5rem;
  }
}

nav li {
  text-align: center;
}

nav a {
  text-decoration: none;
  color: $light-text;
  font-weight: 600;
  padding: 8px 15px;
  border-radius: 25px;
  transition: all 0.3s ease;
  display: block;
  
  &:hover {
    background-color: $primary-color;
    color: $white;
  }
}


main {
  max-width: 1200px;
  margin: 0 auto;
  padding: 2rem 1rem;
  
  @include grid(1fr, 4rem);
}


section {
  margin-bottom: 2rem;
  padding: 2rem;
  background-color: $white;
  border-radius: 15px;
  @include card-shadow;
  @include hover-effect;
}

h2 {
  color: $primary-color;
  margin-bottom: 1.5rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px dashed $accent-color;
  font-size: 2rem;
}

h3 {
  color: $secondary-color;
  margin: 1.5rem 0 0.8rem;
}

// About section grid
#about {
  ul {
    @include grid(repeat(auto-fit, minmax(250px, 1fr)), 1rem);
    margin-top: 1rem;
    list-style: none;
  }
  
  li {
    background-color: lighten($accent-color, 8%);
    padding: 1rem;
    border-radius: 10px;
    border-left: 4px solid $primary-color;
  }
}


#products {
  @include grid(repeat(auto-fit, minmax(300px, 1fr)), 2rem);
}

article {
  background: linear-gradient(to bottom, lighten($accent-color, 8%), $white);
  padding: 1.5rem;
  border-radius: 10px;
  @include card-shadow;
  @include hover-effect;
  
  h3 {
    color: $primary-color;
  }
  
  p:last-child {
    font-weight: bold;
    color: $secondary-color;
    margin-top: 1rem;
    font-size: 1.1rem;
  }
}


#reviews {
  @include grid(1fr, 1.5rem);
}

blockquote {
  background-color: lighten($accent-color, 8%);
  padding: 1.5rem;
  border-radius: 10px;
  border-left: 5px solid $primary-color;
  font-style: italic;
}

cite {
  display: block;
  margin-top: 1rem;
  text-align: right;
  color: $light-text;
  font-weight: 600;
}


#order {
  ol {
    counter-reset: step-counter;
    list-style: none;
    @include grid(1fr, 2rem);
  }
  
  li {
    counter-increment: step-counter;
    padding-left: 3.5rem;
    position: relative;
    
    &::before {
      content: counter(step-counter);
      background-color: $primary-color;
      color: $white;
      font-weight: bold;
      width: 2.5rem;
      height: 2.5rem;
      border-radius: 50%;
      @include flex-center;
      position: absolute;
      left: 0;
      top: 0;
    }
  }
}


#contacts {
  address {
    font-style: normal;
    @include grid(1fr, 1rem);
  }
  
  p {
    display: flex;
    align-items: center;
    
    &::before {
      content: "•";
      color: $primary-color;
      font-weight: bold;
      margin-right: 10px;
    }
  }
}


a {
  color: $primary-color;
  text-decoration: none;
  transition: color 0.3s ease;
  
  &:hover {
    color: $secondary-color;
    text-decoration: underline;
  }
}


footer {
  background: linear-gradient(135deg, $light-color 0%, $accent-color 100%);
  text-align: center;
  padding: 2rem 1rem;
  margin-top: 3rem;
  color: $light-text;
  
  @include grid(1fr, 1rem);
  
  p {
    margin-bottom: 0;
  }
  
  a {
    margin: 0 10px;
    font-weight: 600;
  }
}


@media (max-width: 768px) {
  header h1 {
    font-size: 2.2rem;
  }
  
  section {
    padding: 1.5rem;
  }
  
  #about ul,
  #products {
    grid-template-columns: 1fr;
  }
  
  nav ul {
    grid-template-columns: repeat(2, 1fr);
    
    @media (max-width: 480px) {
      grid-template-columns: 1fr;
    }
  }
  
  #order li {
    padding-left: 2.5rem;
    
    &::before {
      width: 2rem;
      height: 2rem;
    }
  }
}

// Large screens
@media (min-width: 1200px) {
  #products {
    grid-template-columns: repeat(3, 1fr);
  }
  
  #about ul {
    grid-template-columns: repeat(2, 1fr);
  }
}
