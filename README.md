<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IPPALIT - Поиск автозапчастей</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
            background-image: url('background.jpg');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            background-attachment: fixed;
        }

        header {
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 50px 0;
            text-align: center;
            margin-bottom: 20px;
        }

        header h1 {
            font-size: 3rem;
            margin: 0;
        }

        header p {
            font-size: 1.2rem;
        }

        nav {
            background-color: rgba(0, 0, 0, 0.7);
            padding: 15px 0;
            text-align: center;
        }

        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
        }

        nav a:hover {
            text-decoration: underline;
        }

        .container {
            max-width: 1000px;
            margin: 50px auto;
            padding: 40px;
            background: rgba(0, 0, 0, 0.5);
            border-radius: 15px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
            backdrop-filter: blur(10px);
            color: #fff;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 0.8s forwards;
        }

        .container:hover {
            transform: translateY(-10px);
            box-shadow: 0 6px 30px rgba(0, 0, 0, 0.2);
        }

        .container:nth-child(1) {
            animation-delay: 0.2s;
        }

        .container:nth-child(2) {
            animation-delay: 0.4s;
        }

        .container:nth-child(3) {
            animation-delay: 0.6s;
        }

        .container:nth-child(4) {
            animation-delay: 0.8s;
        }

        @keyframes fadeInUp {
            0% {
                opacity: 0;
                transform: translateY(30px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #fff;
        }

        .cta {
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            text-align: center;
            padding: 30px;
            margin: 50px 0;
            border-radius: 10px;
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.1);
        }

        .cta h2 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        .cta p {
            font-size: 1.2rem;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            font-weight: bold;
            margin-bottom: 5px;
        }

        .form-group input, .form-group textarea, .form-group button {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 8px;
            font-size: 1rem;
            margin-bottom: 15px;
        }

        .form-group button {
            background-color: #333;
            color: white;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .form-group button:hover {
            background-color: #555;
        }

        footer {
            text-align: center;
            padding: 30px;
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
        }

        footer p {
            font-size: 1.1rem;
        }

        .contacts-list {
            list-style-type: none;
            padding: 0;
        }

        .contacts-list li {
            margin-bottom: 15px;
        }

        .review-link {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            margin-bottom: 20px;
        }

        .review-link img {
            width: 30px;
            height: 30px;
            border-radius: 50%;
            cursor: pointer;
        }

        .review-link a {
            font-size: 20px;
            color: #fff;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        .review-link a:hover {
            color: #f39c12;
        }

        .review-link i {
            font-size: 30px;
            color: #f39c12;
        }

        .cta-link {
            color: white;
            background-color: #333;
            padding: 10px 20px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s ease;
        }

        .cta-link:hover {
            background-color: #555;
        }

        .phone-link {
            color: white;
            transition: color 0.3s ease;
        }

        .phone-link:hover {
            color: #f39c12;
        }

        /* Aдаптивные стили */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }

            header p {
                font-size: 1rem;
            }

            nav a {
                font-size: 1rem;
                margin: 0 10px;
            }

            .cta h2 {
                font-size: 2rem;
            }

            .cta p {
                font-size: 1rem;
            }

            .container {
                padding: 20px;
                margin: 20px;
            }

            .container h2 {
                font-size: 1.5rem;
            }

            .review-link a {
                font-size: 18px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>IPPALIT</h1>
        <p>Поиск и подбор автозапчастей быстро и надёжно</p>
    </header>
    <nav>
        <a href="#about">О нас</a>
        <a href="#services">Наши услуги</a>
        <a href="#request">Оставить заявку</a>
        <a href="#reviews">Отзывы</a>
        <a href="#contacts">Контакты</a>
    </nav>

    <div class="container" id="about">
        <h2>О нас</h2>
        <p>Мы — команда профессионалов, занимающаяся подбором и поставкой автозапчастей на протяжении более 10 лет...</p>
        <p>Мы активно расширяем свою деятельность на территории новых регионов — Херсонская и Запорожская области...</p>
    </div>

    <div class="container" id="services">
        <h2>Наши услуги</h2>
        <h3>Быстрый поиск и подбор новых и б/у запчастей</h3>
        <p>- Удобный сервис для всех.</p>
        <h3>Распознание VIN с фотографии СТС</h3>
        <p>- Просто пришлите фото, бот запросит оставшуюся информацию.</p>
    </div>

    <div class="cta">
        <h2>Акция!</h2>
        <p>Первая заявка бесплатно!</p>
        <p>Оформите поиск запчасти прямо сейчас и получите скидку 10% на следующую заявку.</p>
    </div>

    <div class="container" id="request">
        <h2>Оставьте заявку</h2>
        <div class="review-link">
            <i class="fas fa-hand-point-right"></i>
            <a href="https://t.me/ippalitzapchasti" target="_blank">Перейти для оформления заявки</a>
        </div>
    </div>

    <div class="container" id="reviews">
        <h2>Отзывы наших клиентов</h2>
        <p>Здесь будут отзывы наших клиентов.</p>
        <div class="review-link">
            <i class="fas fa-comment-dots"></i>
            <a href="javascript:void(0);" onclick="alert('Ваш отзыв принят!')">Оставить отзыв</a>
        </div>
    </div>

    <div class="container" id="contacts">
        <h2>Контакты</h2>
        <ul class="contacts-list">
            <li><strong>Пункт выдачи:</strong> Дудчино, Новая Каховка</li>
            <li><strong>Телефон:</strong> <a href="tel:+79901744516" class="phone-link">+7 (990) 174-45-16</a> (Татьяна)</li>
            <li><strong>Менеджер ИППОЛИТ:</strong> <a href="tel:+79901658140" class="phone-link">+7 990 165 8140</a></li>
            <li><strong>Telegram:</strong> <a href="https://t.me/ippalitzapchasti" class="phone-link" target="_blank">@ippalitzapchasti</a></li>
        </ul>
    </div>

    <footer>
        <p>&copy; 2025 IPPALIT - Все права защищены</p>
    </footer>
</body>
</html>
