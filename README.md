<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Домнин Вячеслав Игоревич - Портфолио</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            color: #333;
        }
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        header {
            background-color: #3498db;
            color: white;
            text-align: center;
            padding: 30px 0;
            margin-bottom: 30px;
        }
        h1 {
            margin: 0;
            font-size: 2.5em;
        }
        .subtitle {
            font-size: 1.2em;
            margin-top: 10px;
        }
        .services {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            margin-bottom: 40px;
        }
        .service-card {
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 20px;
            background-color: #f9f9f9;
            transition: transform 0.3s;
        }
        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        .service-card h3 {
            margin-top: 0;
            color: #3498db;
        }
        .service-card p {
            margin-bottom: 20px;
        }
        .btn {
            display: inline-block;
            background-color: #3498db;
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
            cursor: pointer;
            border: none;
        }
        .btn:hover {
            background-color: #2980b9;
        }
        .about {
            background-color: #f4f4f4;
            padding: 30px;
            border-radius: 8px;
            margin-bottom: 30px;
        }
        .skills {
            margin-bottom: 30px;
        }
        .skills ul {
            list-style-type: none;
            padding-left: 20px;
        }
        .skills li {
            margin-bottom: 5px;
            position: relative;
        }
        .skills li:before {
            content: "•";
            color: #3498db;
            font-weight: bold;
            position: absolute;
            left: -15px;
        }
        .order-form {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 0 20px rgba(0,0,0,0.2);
            z-index: 1000;
            width: 90%;
            max-width: 500px;
        }
        .overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.5);
            z-index: 999;
        }
        .close-btn {
            position: absolute;
            top: 10px;
            right: 10px;
            cursor: pointer;
            font-size: 1.5em;
        }
        form div {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        textarea {
            height: 100px;
        }
        /* Медиа-запросы для адаптивности */
        @media (max-width: 768px) {
            .services {
                grid-template-columns: 1fr;
            }
            .service-card {
                margin-bottom: 15px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Домнин Вячеслав Игоревич</h1>
            <div class="subtitle">Программист, инженер, разработчик решений</div>
        </div>
    </header>
    <div class="container">
        <section class="services">
            <div class="service-card">
                <h3>Telegram-боты</h3>
                <p>Разработка ботов любой сложности — от простых информационных до сложных с интеграцией БД, API и бизнес-логикой.</p>
                <button class="btn" onclick="openOrderForm('Telegram-боты')">Заказать</button>
            </div>
            <div class="service-card">
                <h3>Сайты</h3>
                <p>Создание сайтов различной сложности: от простых лендингов до комплексных веб-приложений с базами данных.</p>
                <button class="btn" onclick="openOrderForm('Сайты')">Заказать</button>
            </div>
            <div class="service-card">
                <h3>Arduino-проекты</h3>
                <p>Разработка устройств на Arduino, проектирование электронных схем, написание программного кода.</p>
                <button class="btn" onclick="openOrderForm('Arduino-проекты')">Заказать</button>
            </div>
            <div class="service-card">
                <h3>Чертежи и 3D-модели</h3>
                <p>Создание технических чертежей, 3D-моделей и документации в программе Компас.</p>
                <button class="btn" onclick="openOrderForm('Чертежи и 3D-модели')">Заказать</button>
            </div>
            <div class="service-card">
                <h3>Конструкторские проекты</h3>
                <p>Разработка инженерных и конструкторских решений, включая сборки, спецификации и документацию.</p>
                <button class="btn" onclick="openOrderForm('Конструкторские проекты')">Заказать</button>
            </div>
            <div class="service-card">
                <h3>Исследовательские работы</h3>
                <p>Подготовка проектов для школы, конкурсов и научных мероприятий.</p>
                <button class="btn" onclick="openOrderForm('Исследовательские работы')">Заказать</button>
            </div>
            <div class="service-card">
                <h3>Python-приложения</h3>
                <p>Разработка десктопных приложений с графическим интерфейсом, логикой и подключением к базам данных.</p>
                <button class="btn" onclick="openOrderForm('Python-приложения')">Заказать</button>
            </div>
            <div class="service-card">
                <h3>Другое</h3>
                <p>Любые другие проекты в области программирования, инженерии и автоматизации.</p>
                <button class="btn" onclick="openOrderForm('Другое')">Заказать</button>
            </div>
        </section>
        <section class="about">
            <h2>Обо мне</h2>
            <p>Начинающий программист с 7-летним опытом работы на Python и 2-летним — на PHP. Прошёл курсы робототехники в колледже "СТАНКИН", призёр конкурса "Инженеры будущего". Дополнительно владею C++ (в том числе для Arduino) и Компас (чертежи, сборки, спецификации). Диплом с отличием по профессии «Чертежник-конструктор».</p>
            <p>Возраст: 16 лет</p>
            <div class="skills">
                <h3>Навыки:</h3>
                <ul>
                    <li>Python, PHP, C++, Arduino</li>
                    <li>Веб-разработка, работа с базами данных</li>
                    <li>Моделирование в Компас</li>
                    <li>Робототехника</li>
                </ul>
            </div>
            <h3>Чем я занимаюсь?</h3>
            <p>Я создаю цифровые и инженерные решения под задачи любой сложности.</p>
            <h4>👨‍💻 Программирование и веб-разработка</h4>
            <p>Telegram-боты любой сложности (от простых до с интеграцией БД, API и логикой)</p>
            <p><strong>Сайты:</strong></p>
            <ul>
                <li>Промо-страницы и лендинги</li>
                <li>Сайты со средней логикой и базой данных</li>
                <li>Сложные веб-проекты (интернет-магазины, учётные системы, админки)</li>
            </ul>
            <h4>🤖 Инженерия и исследования</h4>
            <ul>
                <li>Arduino-проекты (разработка на C++)</li>
                <li>Чертежи и 3D-модели в Компас</li>
                <li>Конструкторские проекты (сборки, спецификации и т.д.)</li>
                <li>Школьные и конкурсные инженерные проекты</li>
                <li>Исследовательские работы на заданную тему</li>
            </ul>
            <h4>🛠 Приложения и автоматизация</h4>
            <ul>
                <li>Десктопные приложения на Python (с графикой, логикой, подключением к БД)</li>
                <li>Автоматизация рутинных задач (боты, скрипты, мини-программы)</li>
            </ul>
        </section>
    </div>
    <div class="overlay" id="overlay"></div>
    <div class="order-form" id="orderForm">
        <div class="close-btn" onclick="closeOrderForm()">×</div>
        <h2>Заказать услугу</h2>
        <p id="selectedService"></p>
        <form id="contactForm">
            <div>
                <label for="name">Имя:</label>
                <input type="text" id="name" name="name" required>
            </div>
            <div>
                <label for="request">Что нужно:</label>
                <textarea id="request" name="request" required></textarea>
            </div>
            <input type="hidden" id="service-input" name="service" value="">
            <button type="submit" class="btn">Отправить</button>
        </form>
    </div>
    <script>
        // Функции для работы с формой заказа
        function openOrderForm(service) {
            document.getElementById('selectedService').textContent = 'Выбранная услуга: ' + service;
            document.getElementById('service-input').value = service;
            document.getElementById('overlay').style.display = 'block';
            document.getElementById('orderForm').style.display = 'block';
        }

        function closeOrderForm() {
            document.getElementById('overlay').style.display = 'none';
            document.getElementById('orderForm').style.display = 'none';
        }

        // Обработка отправки формы
        document.addEventListener('DOMContentLoaded', function() {
            document.getElementById('contactForm').addEventListener('submit', function(e) {
                e.preventDefault();
                
                // Получаем данные из формы
                const name = document.getElementById('name').value;
                const request = document.getElementById('request').value;
                const service = document.getElementById('service-input').value;
                
                // Вывод сообщения об отправке (в простой версии без сервера)
                alert('Спасибо! Ваша заявка принята. Мы свяжемся с вами в ближайшее время.');
                
                // Очищаем форму и закрываем её
                document.getElementById('name').value = '';
                document.getElementById('request').value = '';
                closeOrderForm();
            });
        });
    </script>
</body>
</html> 
