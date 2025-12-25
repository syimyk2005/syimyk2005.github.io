<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Syimyk - Java Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            text-align: center;
            padding: 80px 20px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            margin-bottom: 40px;
            box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
            border: 1px solid rgba(255, 255, 255, 0.18);
        }

        .avatar {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            margin: 0 auto 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }

        h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        .subtitle {
            font-size: 1.3em;
            opacity: 0.9;
            margin-bottom: 20px;
        }

        .tagline {
            font-style: italic;
            font-size: 1.1em;
            opacity: 0.8;
            margin-top: 20px;
        }

        .section {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            margin-bottom: 30px;
            box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
            border: 1px solid rgba(255, 255, 255, 0.18);
            transition: transform 0.3s ease;
        }

        .section:hover {
            transform: translateY(-5px);
        }

        h2 {
            font-size: 2em;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .skill-category {
            background: rgba(255, 255, 255, 0.15);
            padding: 20px;
            border-radius: 15px;
            transition: all 0.3s ease;
        }

        .skill-category:hover {
            background: rgba(255, 255, 255, 0.25);
            transform: scale(1.05);
        }

        .skill-category h3 {
            margin-bottom: 15px;
            font-size: 1.3em;
        }

        .tech-badge {
            display: inline-block;
            background: rgba(255, 255, 255, 0.2);
            padding: 8px 15px;
            border-radius: 20px;
            margin: 5px;
            font-size: 0.9em;
            transition: all 0.3s ease;
        }

        .tech-badge:hover {
            background: rgba(255, 255, 255, 0.35);
            transform: scale(1.1);
        }

        .goals {
            list-style: none;
        }

        .goals li {
            padding: 15px;
            margin: 10px 0;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            border-left: 4px solid #fff;
            transition: all 0.3s ease;
        }

        .goals li:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateX(10px);
        }

        .contact-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 30px;
        }

        .contact-btn {
            background: rgba(255, 255, 255, 0.2);
            color: #fff;
            text-decoration: none;
            padding: 15px 30px;
            border-radius: 30px;
            font-weight: bold;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .contact-btn:hover {
            background: rgba(255, 255, 255, 0.35);
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }

        .philosophy {
            text-align: center;
            font-size: 2em;
            font-weight: bold;
            padding: 40px;
            background: rgba(0, 0, 0, 0.2);
            border-radius: 15px;
            margin: 20px 0;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        footer {
            text-align: center;
            padding: 40px;
            opacity: 0.8;
        }

        @media (max-width: 768px) {
            h1 {
                font-size: 2em;
            }

            .subtitle {
                font-size: 1em;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="avatar">👨‍💻</div>
            <h1>Syimyk</h1>
            <div class="subtitle">
                💻 Junior Java Developer | ☕ Java Enthusiast<br>
                🚀 Exploring CI/CD, Microservices & Scalable Backend Systems
            </div>
            <div class="tagline">"Code. Learn. Automate. Repeat."</div>
        </header>

        <div class="section">
            <h2>🎯 О себе</h2>
            <p style="font-size: 1.1em; line-height: 1.8;">
                Я увлеченный разработчик, который постоянно совершенствует свои навыки в мире backend-разработки. 
                Моя цель — стать <strong>Software Engineer в Big Tech</strong> компании, создавая высоконагруженные и надежные системы.
            </p>
            <ul class="goals" style="margin-top: 20px;">
                <li>🔹 Изучаю <strong>Spring Boot, Spring Security</strong> — для создания безопасных приложений</li>
                <li>🔹 Осваиваю <strong>Kafka, gRPC</strong> — для построения микросервисной архитектуры</li>
                <li>🔹 Практикую <strong>Docker, CI/CD</strong> — для автоматизации и эффективной разработки</li>
                <li>🔹 Работаю с <strong>Redis, PostgreSQL</strong> — для работы с данными на высокой скорости</li>
            </ul>
        </div>

        <div class="section">
            <h2>🛠️ Технологический стек</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>💡 Backend</h3>
                    <div class="tech-badge">Java 21</div>
                    <div class="tech-badge">Spring Boot</div>
                    <div class="tech-badge">Spring Security</div>
                    <div class="tech-badge">gRPC</div>
                    <div class="tech-badge">Kafka</div>
                    <div class="tech-badge">Redis</div>
                </div>
                <div class="skill-category">
                    <h3>🗄️ Базы данных</h3>
                    <div class="tech-badge">PostgreSQL</div>
                    <div class="tech-badge">MySQL</div>
                    <div class="tech-badge">MongoDB</div>
                </div>
                <div class="skill-category">
                    <h3>⚙️ DevOps & Tools</h3>
                    <div class="tech-badge">Docker</div>
                    <div class="tech-badge">GitHub Actions</div>
                    <div class="tech-badge">Jenkins</div>
                    <div class="tech-badge">Maven</div>
                    <div class="tech-badge">Git</div>
                </div>
            </div>
        </div>

        <div class="section">
            <h2>🖥️ Рабочие среды</h2>
            <div style="text-align: center; margin-top: 20px;">
                <div class="tech-badge" style="font-size: 1.1em;">Ubuntu</div>
                <div class="tech-badge" style="font-size: 1.1em;">Arch Linux</div>
                <div class="tech-badge" style="font-size: 1.1em;">Windows</div>
            </div>
        </div>

        <div class="section">
            <h2>🎓 Мои принципы</h2>
            <ul class="goals">
                <li>📖 <strong>Постоянное обучение</strong> — технологии развиваются, и я развиваюсь вместе с ними</li>
                <li>🔄 <strong>Автоматизация</strong> — если задачу можно автоматизировать, её нужно автоматизировать</li>
                <li>🎯 <strong>Качество кода</strong> — чистый код — это инвестиция в будущее проекта</li>
                <li>🤝 <strong>Командная работа</strong> — лучшие решения рождаются в коллаборации</li>
            </ul>
        </div>

        <div class="philosophy">
            💼 Открыт для интересных проектов и сотрудничества!
        </div>

        <div class="section">
            <h2>📫 Связаться со мной</h2>
            <div class="contact-links">
                <a href="#" class="contact-btn">📱 Telegram</a>
                <a href="#" class="contact-btn">✉️ Email</a>
                <a href="#" class="contact-btn">💼 LinkedIn</a>
                <a href="#" class="contact-btn">🐙 GitHub</a>
            </div>
        </div>

        <footer>
            <p>⭐ Создано с passion и Java ☕</p>
        </footer>
    </div>
</body>
</html>
