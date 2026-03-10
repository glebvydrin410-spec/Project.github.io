<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Классный архив: наши работы</title>
    <link rel="stylesheet" href="style.css">
    <link rel="icon" href="favicon.ico" type="image/x-icon">
</head>
<body>
    <header>
        <div class="logo">
            <h1>📚 Классный архив</h1>
            <p>Сайт для наших учебных работ</p>
        </div>
        <nav>
            <a href="index.html">Главная</a>
            <a href="subjects.html">Предметы</a>
            <a href="gallery.html">Галерея</a>
            <a href="about.html">О нас</a>
            <a href="contact.html">Контакты</a>
        </nav>
    </header>

    <main>
        <section class="intro">
            <h2>Добро пожаловать!</h2>
            <p>Здесь мы храним наши лучшие классные работы, проекты и творческие задания. Вы можете найти материалы по предметам, авторам или дате.</p>
        </section>

        <section class="latest-works">
            <h2>Последние работы</h2>
            <div class="work-card">
                <h3>Проект: Разработка простого веб сайта</h3>
                <p>Информатика, 9 класс</p>
                <p><em>Автор: Выдрин Глеб</em></p>
                <a href="#">Смотреть работу</a>
            </div>
            <!-- другие карточки -->
        </section>
    </main>

    <footer>
        <p>© 2026 Архив работ 9В класса. Все права защищены.</p>
        <p>Сайт создан в учебных целях.</p>
    </footer>
</body>
</html>

/* style.css — основной стиль для архива класса */

/* Сброс отступов и базовые настройки */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f9f7f3;
    color: #2e3b4e;
    line-height: 1.6;
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

/* Шапка */
header {
    background-color: #3b5b7c;
    color: white;
    padding: 1.5rem 2rem;
    text-align: center;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
}

.logo h1 {
    font-size: 2.2rem;
    letter-spacing: 1px;
    margin-bottom: 0.25rem;
}

.logo p {
    font-style: italic;
    opacity: 0.9;
}

/* Навигация */
nav {
    margin-top: 1rem;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 1rem;
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: 500;
    padding: 0.5rem 1rem;
    border-radius: 30px;
    background-color: rgba(255,255,255,0.15);
    transition: all 0.3s ease;
}

nav a:hover {
    background-color: rgba(255,255,255,0.3);
    transform: scale(1.05);
}

/* Основной контент */
main {
    flex: 1;
    max-width: 1200px;
    margin: 2rem auto;
    padding: 0 2rem;
    width: 100%;
}

section {
    margin-bottom: 3rem;
}

h2 {
    font-size: 2rem;
    color: #2c3e50;
    border-bottom: 3px solid #d4af37;
    padding-bottom: 0.5rem;
    margin-bottom: 2rem;
    display: inline-block;
}

/* Приветственный блок */
.intro {
    background-color: #e8f0fe;
    padding: 2rem;
    border-radius: 16px;
    text-align: center;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
}

.intro p {
    font-size: 1.2rem;
    max-width: 700px;
    margin: 1rem auto 0;
}

/* Карточки работ */
.latest-works {
    margin-top: 2rem;
}

.work-card {
    background: white;
    border-radius: 20px;
    padding: 1.8rem;
    margin-bottom: 1.5rem;
    box-shadow: 0 10px 20px rgba(0,0,0,0.03);
    border: 1px solid #e0dcd5;
    transition: transform 0.2s, box-shadow 0.2s;
}

.work-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.1);
}

.work-card h3 {
    font-size: 1.6rem;
    color: #3b5b7c;
    margin-bottom: 0.5rem;
}

.work-card p {
    margin-bottom: 0.75rem;
    color: #4a5b6e;
}

.work-card em {
    color: #7f8c8d;
    font-style: italic;
}

.work-card a {
    display: inline-block;
    margin-top: 0.5rem;
    color: #d4af37;
    font-weight: 600;
    text-decoration: none;
    border-bottom: 2px solid transparent;
    transition: border-color 0.2s;
}

.work-card a:hover {
    border-bottom-color: #d4af37;
}

/* Подвал */
footer {
    background-color: #2e3b4e;
    color: #ccc;
    text-align: center;
    padding: 1.5rem;
    font-size: 0.95rem;
    border-top: 4px solid #d4af37;
}

footer p {
    margin: 0.25rem 0;
}

/* Адаптивность */
@media (max-width: 600px) {
    header {
        padding: 1rem;
    }
    .logo h1 {
        font-size: 1.8rem;
    }
    nav {
        flex-direction: column;
        align-items: center;
    }
    nav a {
        width: 80%;
        text-align: center;
    }
    .intro {
        padding: 1.5rem;
    }
    h2 {
        font-size: 1.6rem;
    }
}
