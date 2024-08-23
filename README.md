<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CV Axilot</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        /* Global Styles */
        html {
            scroll-behavior: smooth;
        }
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f4f7f6;
            color: #333;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            line-height: 1.6;
        }

        /* Header */
        header {
            background: linear-gradient(90deg, #0d47a1, #42a5f5);
            color: white;
            text-align: center;
            padding: 50px 0;
            position: relative;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
            animation: slideDown 1s ease-out;
        }
        header h1 {
            font-size: 2.5rem;
            font-weight: 700;
            letter-spacing: 2px;
            text-transform: uppercase;
        }

        /* Navigation */
        nav {
            background: white;
            padding: 20px 0;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        nav a {
            color: #333;
            margin: 0 15px;
            text-decoration: none;
            font-weight: 500;
            font-size: 18px;
            transition: color 0.3s ease;
            padding: 10px 15px;
            position: relative;
        }
        nav a:hover {
            color: #42a5f5;
        }
        nav a::after {
            content: '';
            display: block;
            width: 0;
            height: 2px;
            background: #42a5f5;
            transition: width 0.3s;
            position: absolute;
            bottom: -5px;
            left: 50%;
            transform: translateX(-50%);
        }
        nav a:hover::after {
            width: 100%;
        }

        /* Main Content */
        main {
            padding: 40px 20px;
            max-width: 1000px;
            margin: auto;
        }
        .section {
            margin-bottom: 60px;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 0.8s forwards ease-in-out;
            animation-delay: 0.3s;
        }
        .section:nth-child(even) {
            animation-delay: 0.5s;
        }
        .section h2 {
            font-size: 2rem;
            color: #0d47a1;
            margin-bottom: 20px;
            text-transform: uppercase;
            border-bottom: 2px solid #42a5f5;
            display: inline-block;
            padding-bottom: 5px;
        }
        .section p {
            margin-bottom: 20px;
            font-size: 1.1rem;
            line-height: 1.8;
        }

        /* Skills */
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        .skill-bar {
            flex: 1;
            background: #e0e0e0;
            border-radius: 50px;
            overflow: hidden;
            position: relative;
            height: 30px;
            margin-bottom: 10px;
        }
        .skill-bar-fill {
            background: linear-gradient(90deg, #42a5f5, #0d47a1);
            height: 100%;
            width: 0;
            border-radius: 50px;
            transition: width 1.5s ease-in-out;
        }
        .skill-title {
            font-size: 1.1rem;
            color: #333;
            margin-bottom: 5px;
            display: flex;
            align-items: center;
        }
        .skill-title i {
            margin-right: 10px;
            color: #42a5f5;
        }

        /* Profile Image */
        .profile-photo {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 20px;
            transition: transform 0.3s ease;
        }
        .profile-photo:hover {
            transform: scale(1.05);
        }

        /* Footer */
        footer {
            background-color: #0d47a1;
            color: white;
            text-align: center;
            padding: 30px 0;
            box-shadow: 0 -4px 10px rgba(0, 0, 0, 0.2);
            margin-top: 40px;
            position: relative;
            animation: fadeInUp 1s ease-in-out;
        }
        footer p {
            margin: 0;
            font-size: 1rem;
        }

        /* Keyframes */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-100%);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Axilot's Portfolio</h1>
    </header>

    <nav>
        <a href="#profile">Profile</a>
        <a href="#education">Education</a>
        <a href="#experience">Experience</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
    </nav>

    <main>
        <section id="profile" class="section">
            <img src="★ _ _ Kaoruko Waguri.jpeg" alt="Axilot's Photo" class="profile-photo">
            <h2>Profile</h2>
            <p>Hello, I am Axilot, a passionate web developer with a deep interest in building modern and responsive web applications. I am always eager to learn and implement new technologies in my work.</p>
        </section>

        <section id="education" class="section">
            <h2>Education</h2>
            <p>I hold a Bachelor's degree in Computer Science from Universitas Indonesia, where I graduated with honors.</p>
        </section>

        <section id="experience" class="section">
            <h2>Experience</h2>
            <p>Currently, I work as a Full Stack Developer at PT XYZ, focusing on building scalable web applications.</p>
        </section>

        <section id="skills" class="section">
            <h2>Skills</h2>
            <div class="skills-container">
                <div class="skill-title"><i class="fab fa-html5"></i> HTML5</div>
                <div class="skill-bar">
                    <div class="skill-bar-fill" style="width: 95%;"></div>
                </div>
                <div class="skill-title"><i class="fab fa-js-square"></i> JavaScript</div>
                <div class="skill-bar">
                    <div class="skill-bar-fill" style="width: 90%;"></div>
                </div>
            </div>
        </section>

        <section id="contact" class="section">
            <h2>Contact</h2>
            <p>Email: axilot@example.com</p>
            <p>Phone: +62 812 3456 7890</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Axilot. All rights reserved.</p>
    </footer>

    <script>
        // Smooth scroll with animation
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                document.querySelector(targetId).scrollIntoView({
                    behavior: 'smooth',
                    block: 'center'
                });
            });
        });

        // Animate skill bars on scroll
        window.addEventListener('scroll', function() {
            const skills = document.querySelectorAll('.skill-bar-fill');
            skills.forEach(skill => {
                const skillPos = skill.getBoundingClientRect().top;
                const windowHeight = window.innerHeight;
                if (skillPos < windowHeight - 100) {
                    skill.style.width = skill.getAttribute('style').split('width: ')[1];
                }
            });
        });
    </script>
</body>
</html>
