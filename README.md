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




STYLE.CSS

 * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    background-color: #fff9f5;
    color: #5a3e36;
    line-height: 1.6;
}

header {
    background: linear-gradient(135deg, #f8e3e3 0%, #f5d0d0 100%);
    padding: 2rem 1rem;
    text-align: center;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    position: sticky;
    top: 0;
    z-index: 100;
}

header h1 {
    font-size: 3rem;
    color: #d46a6a;
    margin-bottom: 0.5rem;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
}

header p {
    font-size: 1.2rem;
    color: #8c5e5e;
    margin-bottom: 1.5rem;
    font-style: italic;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style: none;
    flex-wrap: wrap;
}

nav li {
    margin: 0 15px;
}

nav a {
    text-decoration: none;
    color: #8c5e5e;
    font-weight: 600;
    padding: 8px 15px;
    border-radius: 25px;
    transition: all 0.3s ease;
}

nav a:hover {
    background-color: #d46a6a;
    color: white;
}

main {
    max-width: 1200px;
    margin: 0 auto;
    padding: 2rem 1rem;
}

section {
    margin-bottom: 4rem;
    padding: 2rem;
    background-color: white;
    border-radius: 15px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
    transition: transform 0.3s ease;
}

section:hover {
    transform: translateY(-5px);
}

h2 {
    color: #d46a6a;
    margin-bottom: 1.5rem;
    padding-bottom: 0.5rem;
    border-bottom: 2px dashed #f5d0d0;
    font-size: 2rem;
}

h3 {
    color: #b85c5c;
    margin: 1.5rem 0 0.8rem;
}

p {
    margin-bottom: 1rem;
}

ul, ol {
    margin-left: 1.5rem;
    margin-bottom: 1rem;
}

li {
    margin-bottom: 0.5rem;
}

#about ul {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1rem;
    margin-top: 1rem;
}

#about li {
    background-color: #fef5f5;
    padding: 1rem;
    border-radius: 10px;
    list-style: none;
    margin-left: 0;
    border-left: 4px solid #d46a6a;
}

#products {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

article {
    background: linear-gradient(to bottom, #fff9f9, #fff);
    padding: 1.5rem;
    border-radius: 10px;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
    transition: all 0.3s ease;
}

article:hover {
    transform: scale(1.03);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
}

article h3 {
    color: #d46a6a;
}

article p:last-child {
    font-weight: bold;
    color: #b85c5c;
    margin-top: 1rem;
    font-size: 1.1rem;
}

blockquote {
    background-color: #fef5f5;
    padding: 1.5rem;
    border-radius: 10px;
    margin-bottom: 1.5rem;
    border-left: 5px solid #d46a6a;
    font-style: italic;
}

cite {
    display: block;
    margin-top: 1rem;
    text-align: right;
    color: #8c5e5e;
    font-weight: 600;
}

#order ol {
    counter-reset: step-counter;
    list-style: none;
}

#order li {
    counter-increment: step-counter;
    margin-bottom: 2rem;
    padding-left: 3.5rem;
    position: relative;
}

#order li:before {
    content: counter(step-counter);
    background-color: #d46a6a;
    color: white;
    font-weight: bold;
    width: 2.5rem;
    height: 2.5rem;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    position: absolute;
    left: 0;
    top: 0;
}

address {
    font-style: normal;
}

address p {
    margin-bottom: 1rem;
    display: flex;
    align-items: center;
}

address p:before {
    content: "•";
    color: #d46a6a;
    font-weight: bold;
    margin-right: 10px;
}

a {
    color: #d46a6a;
    text-decoration: none;
    transition: color 0.3s ease;
}

a:hover {
    color: #b85c5c;
    text-decoration: underline;
}

footer {
    background: linear-gradient(135deg, #f8e3e3 0%, #f5d0d0 100%);
    text-align: center;
    padding: 2rem 1rem;
    margin-top: 3rem;
    color: #8c5e5e;
}

footer p {
    margin-bottom: 1rem;
}

footer a {
    margin: 0 10px;
    font-weight: 600;
}

@media (max-width: 768px) {
    header h1 {
        font-size: 2.2rem;
    }
    
    nav ul {
        flex-direction: column;
        align-items: center;
    }
    
    nav li {
        margin: 5px 0;
    }
    
    section {
        padding: 1.5rem;
    }
    
    #about ul {
        grid-template-columns: 1fr;
    }
    
    #products {
        grid-template-columns: 1fr;
    }
}
