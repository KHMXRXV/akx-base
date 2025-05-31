<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Название галереи</title>
    <style>
        /* Основные стили */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            background-color: #f8f8f8;
            color: #333;
            line-height: 1.6;
        }
        
        /* Шапка */
        header {
            background-color: #222;
            color: white;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 1.5rem;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: #ccc;
        }
        
        /* Основной контент */
        main {
            padding: 2rem 0;
        }
        
        .gallery-title {
            text-align: center;
            margin-bottom: 2rem;
        }
        
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .gallery-item {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .gallery-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .gallery-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            display: block;
        }
        
        .item-info {
            padding: 1rem;
        }
        
        .item-info h3 {
            margin-bottom: 0.5rem;
        }
        
        .item-info p {
            color: #666;
            font-size: 0.9rem;
        }
        
        /* Подвал */
        footer {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 1.5rem 0;
            margin-top: 2rem;
        }
        
        /* Адаптивность */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 1rem;
                justify-content: center;
            }
            
            nav ul li {
                margin: 0 0.75rem;
            }
            
            .gallery-grid {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">Название галереи</div>
                <nav>
                    <ul>
                        <li><a href="#">Главная</a></li>
                        <li><a href="#">Коллекции</a></li>
                        <li><a href="#">О нас</a></li>
                        <li><a href="#">Контакты</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
    
    <main>
        <div class="container">
            <h1 class="gallery-title">Наша галерея</h1>
            
            <div class="gallery-grid">
                <!-- Пример элемента галереи -->
                <div class="gallery-item">
                    <img src="https://via.placeholder.com/300x250" alt="Пример работы">
                    <div class="item-info">
                        <h3>Название работы</h3>
                        <p>Автор: Имя Автора</p>
                        <p>Год: 2023</p>
                    </div>
                </div>
                
                <!-- Дублируем элементы для демонстрации -->
                <div class="gallery-item">
                    <img src="https://via.placeholder.com/300x250" alt="Пример работы">
                    <div class="item-info">
                        <h3>Название работы 2</h3>
                        <p>Автор: Имя Автора</p>
                        <p>Год: 2023</p>
                    </div>
                </div>
                
                <div class="gallery-item">
                    <img src="https://via.placeholder.com/300x250" alt="Пример работы">
                    <div class="item-info">
                        <h3>Название работы 3</h3>
                        <p>Автор: Имя Автора</p>
                        <p>Год: 2023</p>
                    </div>
                </div>
                
                <div class="gallery-item">
                    <img src="https://via.placeholder.com/300x250" alt="Пример работы">
                    <div class="item-info">
                        <h3>Название работы 4</h3>
                        <p>Автор: Имя Автора</p>
                        <p>Год: 2023</p>
                    </div>
                </div>
                
                <div class="gallery-item">
                    <img src="https://via.placeholder.com/300x250" alt="Пример работы">
                    <div class="item-info">
                        <h3>Название работы 5</h3>
                        <p>Автор: Имя Автора</p>
                        <p>Год: 2023</p>
                    </div>
                </div>
                
                <div class="gallery-item">
                    <img src="https://via.placeholder.com/300x250" alt="Пример работы">
                    <div class="item-info">
                        <h3>Название работы 6</h3>
                        <p>Автор: Имя Автора</p>
                        <p>Год: 2023</p>
                    </div>
                </div>
            </div>
        </div>
    </main>
    
    <footer>
        <div class="container">
            <p>&copy; 2023 Название галереи. Все права защищены.</p>
        </div>
    </footer>
</body>
</html>
