<!DOCTYPE html>
<html lang="en">
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

        @media (max-width: 768px) {
            header h1 {
                font-size: 2.5rem;
            }
            header p {
                font-size: 1rem;
            }
            nav a {
                font-size: 0.9rem;
                margin: 0 10px;
            }
            .container {
                padding: 20px;
            }
            h2 {
                font-size: 1.8rem;
            }
            .cta h2 {
                font-size: 2rem;
            }
            .cta p {
                font-size: 1rem;
            }
        }

        @media (max-width: 480px) {
            header h1 {
                font-size: 2rem;
            }
            header p {
                font-size: 0.9rem;
            }
            nav a {
                font-size: 0.8rem;
                margin: 0 5px;
            }
            .container {
                padding: 15px;
            }
            h2 {
                font-size: 1.5rem;
            }
            .cta h2 {
                font-size: 1.8rem;
            }
            .cta p {
                font-size: 0.9rem;
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
        <p>Мы — команда профессионалов...</p>
    </div>

    <div class="container" id="services">
        <h2>Наши услуги</h2>
        <h3>Быстрый поиск и подбор новых и б/у запчастей</h3>
        <p>- Удобный сервис для всех.</p>
        <h3>Распознание VIN с фотографии СТС</h3>
        <p>- Просто пришлите фото...</p>
    </div>

    <div class="cta">
        <h2>Акция!</h2>
        <p>Первая заявка бесплатно!</p>
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
    </div>

    <div class="container" id="contacts">
        <h2>Контакты</h2>
        <ul class="contacts-list">
            <li><strong>Пункт выдачи:</strong> Дудчино...</li>
        </ul>
    </div>

    <footer>
        <p>&copy; 2025 IPPALIT. Все права защищены.</p>
    </footer>
</body>
</html>
