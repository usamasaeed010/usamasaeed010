<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Usama Saeed - Mobile Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #0d1117;
            color: #c9d1d9;
            line-height: 1.6;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        .container {
            display: flex;
            flex-direction: column;
            gap: 30px;
        }
        
        header {
            display: flex;
            align-items: center;
            gap: 25px;
            padding: 20px 0;
            border-bottom: 1px solid #30363d;
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 3px solid #58a6ff;
            object-fit: cover;
        }
        
        .header-text h1 {
            font-size: 2.5rem;
            margin-bottom: 5px;
            color: #f0f6fc;
        }
        
        .header-text h2 {
            font-size: 1.5rem;
            color: #58a6ff;
            margin-bottom: 10px;
        }
        
        .header-text p {
            font-size: 1.1rem;
            max-width: 600px;
        }
        
        .badge {
            display: inline-block;
            background-color: #238636;
            color: white;
            padding: 3px 10px;
            border-radius: 20px;
            font-size: 0.9rem;
            margin-top: 10px;
        }
        
        .stats {
            display: flex;
            gap: 20px;
            margin-top: 10px;
        }
        
        .stat-item {
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        section {
            background-color: #161b22;
            border-radius: 10px;
            padding: 25px;
            border: 1px solid #30363d;
        }
        
        h3 {
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: #f0f6fc;
            border-bottom: 2px solid #58a6ff;
            padding-bottom: 8px;
            display: inline-block;
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .skill-category {
            margin-bottom: 20px;
        }
        
        .skill-category h4 {
            color: #58a6ff;
            margin-bottom: 10px;
            font-size: 1.2rem;
        }
        
        .skill-items {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .skill-item {
            background-color: #21262d;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            border: 1px solid #30363d;
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
        }
        
        .project-card {
            background-color: #21262d;
            border-radius: 10px;
            padding: 20px;
            border: 1px solid #30363d;
            transition: transform 0.3s ease;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            border-color: #58a6ff;
        }
        
        .project-card h4 {
            color: #58a6ff;
            margin-bottom: 10px;
            font-size: 1.2rem;
        }
        
        .project-card p {
            margin-bottom: 15px;
            font-size: 0.95rem;
        }
        
        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 15px;
        }
        
        .tech-tag {
            background-color: #0d1117;
            padding: 4px 10px;
            border-radius: 15px;
            font-size: 0.8rem;
        }
        
        .project-links {
            display: flex;
            gap: 15px;
        }
        
        .btn {
            display: inline-block;
            padding: 8px 15px;
            background-color: #238636;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-size: 0.9rem;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #2ea043;
        }
        
        .btn-outline {
            background-color: transparent;
            border: 1px solid #58a6ff;
            color: #58a6ff;
        }
        
        .btn-outline:hover {
            background-color: rgba(88, 166, 255, 0.1);
        }
        
        .contact-links {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
        }
        
        .contact-link {
            display: flex;
            align-items: center;
            gap: 8px;
            color: #c9d1d9;
            text-decoration: none;
            padding: 10px 15px;
            background-color: #21262d;
            border-radius: 5px;
            border: 1px solid #30363d;
            transition: all 0.3s;
        }
        
        .contact-link:hover {
            background-color: #30363d;
            border-color: #58a6ff;
        }
        
        .contact-link i {
            font-size: 1.2rem;
        }
        
        footer {
            text-align: center;
            padding: 20px 0;
            margin-top: 20px;
            border-top: 1px solid #30363d;
            color: #8b949e;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                text-align: center;
            }
            
            .stats {
                justify-content: center;
            }
            
            .skills-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <div class="container">
        <header>
            <img src="https://avatars.githubusercontent.com/u/12345678?v=4" alt="Profile Picture" class="profile-img">
            <div class="header-text">
                <h1>Usama Saeed</h1>
                <h2>Mobile Application Developer</h2>
                <p>Passionate Mobile Developer specializing in Flutter, Android (Java/Kotlin), and React Native. I build high-quality, performant, and user-friendly mobile applications.</p>
                <span class="badge">Open to opportunities</span>
                <div class="stats">
                    <div class="stat-item">
                        <i class="fas fa-map-marker-alt"></i>
                        <span>Pakistan</span>
                    </div>
                    <div class="stat-item">
                        <i class="fas fa-envelope"></i>
                        <span>usaeed000@gmail.com</span>
                    </div>
                </div>
            </div>
        </header>
        
        <section>
            <h3>Technical Skills</h3>
            <div class="skills-grid">
                <div class="skill-category">
                    <h4>Mobile Development</h4>
                    <div class="skill-items">
                        <span class="skill-item">Flutter</span>
                        <span class="skill-item">Dart</span>
                        <span class="skill-item">Android</span>
                        <span class="skill-item">Kotlin</span>
                        <span class="skill-item">Java</span>
                        <span class="skill-item">React Native</span>
                        <span class="skill-item">iOS</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h4>Backend Development</h4>
                    <div class="skill-items">
                        <span class="skill-item">Spring Boot</span>
                        <span class="skill-item">REST APIs</span>
                        <span class="skill-item">Node.js</span>
                        <span class="skill-item">Firebase</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h4>Databases</h4>
                    <div class="skill-items">
                        <span class="skill-item">MySQL</span>
                        <span class="skill-item">SQLite</span>
                        <span class="skill-item">Firestore</span>
                        <span class="skill-item">MongoDB</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h4>Tools & Technologies</h4>
                    <div class="skill-items">
                        <span class="skill-item">Git</span>
                        <span class="skill-item">Postman</span>
                        <span class="skill-item">Android Studio</span>
                        <span class="skill-item">VS Code</span>
                        <span class="skill-item">Figma</span>
                        <span class="skill-item">Adobe XD</span>
                        <span class="skill-item">Photoshop</span>
                    </div>
                </div>
            </div>
        </section>
        
        <section>
            <h3>Featured Projects</h3>
            <div class="projects-grid">
                <div class="project-card">
                    <h4>E-Commerce Flutter App</h4>
                    <p>A complete e-commerce mobile application built with Flutter and Firebase with features like user authentication, product catalog, shopping cart, and payment integration.</p>
                    <div class="project-tech">
                        <span class="tech-tag">Flutter</span>
                        <span class="tech-tag">Dart</span>
                        <span class="tech-tag">Firebase</span>
                        <span class="tech-tag">Stripe</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="btn">View Code</a>
                        <a href="#" class="btn btn-outline">Live Demo</a>
                    </div>
                </div>
                
                <div class="project-card">
                    <h4>Task Management Android App</h4>
                    <p>Productivity application for task management with features like categories, priorities, reminders, and data synchronization across devices.</p>
                    <div class="project-tech">
                        <span class="tech-tag">Kotlin</span>
                        <span class="tech-tag">Room DB</span>
                        <span class="tech-tag">MVVM</span>
                        <span class="tech-tag">Coroutines</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="btn">View Code</a>
                        <a href="#" class="btn btn-outline">Play Store</a>
                    </div>
                </div>
                
                <div class="project-card">
                    <h4>Social Media React Native App</h4>
                    <p>A cross-platform social media application with real-time messaging, post sharing, and user interaction features.</p>
                    <div class="project-tech">
                        <span class="tech-tag">React Native</span>
                        <span class="tech-tag">Node.js</span>
                        <span class="tech-tag">MongoDB</span>
                        <span class="tech-tag">Socket.io</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="btn">View Code</a>
                        <a href="#" class="btn btn-outline">Live Demo</a>
                    </div>
                </div>
            </div>
        </section>
        
        <section>
            <h3>Experience & Education</h3>
            <div class="skills-grid">
                <div class="skill-category">
                    <h4>Professional Experience</h4>
                    <div class="skill-items">
                        <div class="skill-item" style="display: block; text-align: left; margin-bottom: 15px;">
                            <strong>Mobile App Developer</strong><br>
                            ABC Tech Solutions | 2021 - Present<br>
                            Developed and maintained multiple Flutter and Android applications with 50k+ downloads.
                        </div>
                        <div class="skill-item" style="display: block; text-align: left;">
                            <strong>Android Developer Intern</strong><br>
                            XYZ Innovations | 2020 - 2021<br>
                            Contributed to the development of enterprise Android applications using Java and Kotlin.
                        </div>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h4>Education</h4>
                    <div class="skill-items">
                        <div class="skill-item" style="display: block; text-align: left;">
                            <strong>Bachelor of Computer Science</strong><br>
                            University of Punjab | 2017 - 2021<br>
                            Graduated with honors, focusing on mobile development and software engineering.
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section>
            <h3>Get In Touch</h3>
            <div class="contact-links">
                <a href="https://github.com/usamasaeed010" class="contact-link">
                    <i class="fab fa-github"></i>
                    <span>GitHub</span>
                </a>
                <a href="https://www.linkedin.com/in/usama-saeed-61205b207" class="contact-link">
                    <i class="fab fa-linkedin"></i>
                    <span>LinkedIn</span>
                </a>
                <a href="https://web.facebook.com/profile.php?id=100006136846857" class="contact-link">
                    <i class="fab fa-facebook"></i>
                    <span>Facebook</span>
                </a>
                <a href="https://www.instagram.com/khan_sab_01" class="contact-link">
                    <i class="fab fa-instagram"></i>
                    <span>Instagram</span>
                </a>
                <a href="mailto:usaeed000@gmail.com" class="contact-link">
                    <i class="fas fa-envelope"></i>
                    <span>Email</span>
                </a>
            </div>
        </section>
        
        <footer>
            <p>&copy; 2023 Usama Saeed. All rights reserved.</p>
            <p>Made with ❤️ using HTML & CSS</p>
        </footer>
    </div>
</body>
</html>
