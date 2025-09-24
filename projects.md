---
layout: default
title: Projects
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projects - Zahir Choudhry</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: #f8f9fa;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #667eea;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: #667eea;
        }

        /* Main Content */
        main {
            padding-top: 120px;
            min-height: 100vh;
        }

        .page-header {
            text-align: center;
            padding: 4rem 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            margin-bottom: 4rem;
        }

        .page-title {
            font-size: 3rem;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .page-subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
        }

        /* Projects Grid */
        .projects-section {
            padding: 2rem 0 4rem;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .project-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
        }

        .project-image {
            height: 200px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3rem;
            font-weight: bold;
        }

        .project-content {
            padding: 2rem;
        }

        .project-title {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: #333;
        }

        .project-description {
            color: #666;
            margin-bottom: 1.5rem;
            line-height: 1.6;
        }

        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-bottom: 1.5rem;
        }

        .tech-tag {
            background: #e9ecef;
            color: #495057;
            padding: 0.3rem 0.8rem;
            border-radius: 15px;
            font-size: 0.85rem;
            font-weight: 500;
        }

        .project-links {
            display: flex;
            gap: 1rem;
        }

        .project-link {
            display: inline-block;
            padding: 0.7rem 1.5rem;
            text-decoration: none;
            border-radius: 25px;
            font-weight: 600;
            transition: all 0.3s ease;
            text-align: center;
            flex: 1;
        }

        .primary-link {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }

        .primary-link:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        .secondary-link {
            background: transparent;
            color: #667eea;
            border: 2px solid #667eea;
        }

        .secondary-link:hover {
            background: #667eea;
            color: white;
        }

        /* Coming Soon Section */
        .coming-soon {
            background: white;
            border-radius: 15px;
            padding: 3rem;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            margin-top: 3rem;
        }

        .coming-soon h3 {
            color: #333;
            margin-bottom: 1rem;
            font-size: 1.8rem;
        }

        .coming-soon p {
            color: #666;
            font-size: 1.1rem;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 4rem;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .page-title {
                font-size: 2.5rem;
            }

            .projects-grid {
                grid-template-columns: 1fr;
            }

            .project-links {
                flex-direction: column;
            }
        }

        @media (max-width: 480px) {
            .page-title {
                font-size: 2rem;
            }

            .project-content {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav class="container">
            <div class="logo">Zahir Choudhry</div>
            <ul class="nav-links">
                <li><a href="index.html">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="projects.html">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Main Content -->
    <main>
        <!-- Page Header -->
        <section class="page-header">
            <div class="container">
                <h1 class="page-title">My Projects</h1>
                <p class="page-subtitle">A showcase of my development work, featuring web applications, data analysis tools, and innovative solutions built with modern technologies.</p>
            </div>
        </section>

        <!-- Projects Section -->
        <section class="projects-section">
            <div class="container">
                <div class="projects-grid">
                    <!-- Project 1 -->
                    <div class="project-card">
                        <div class="project-image">🌐</div>
                        <div class="project-content">
                            <h3 class="project-title">Portfolio Website</h3>
                            <p class="project-description">A responsive personal portfolio website built with modern web technologies. Features smooth animations, mobile-first design, and optimized performance. Showcases my journey as a software developer with an elegant, professional interface.</p>
                            <div class="project-tech">
                                <span class="tech-tag">HTML5</span>
                                <span class="tech-tag">CSS3</span>
                                <span class="tech-tag">JavaScript</span>
                                <span class="tech-tag">GitHub Pages</span>
                                <span class="tech-tag">Responsive Design</span>
                            </div>
                            <div class="project-links">
                                <a href="https://zahir-choudhry.github.io" class="project-link primary-link" target="_blank">Live Demo</a>
                                <a href="https://github.com/BiggestZ/zahir-choudhry.github.io" class="project-link secondary-link" target="_blank">GitHub</a>
                            </div>
                        </div>
                    </div>

                    <!-- Project 2 -->
                    <div class="project-card">
                        <div class="project-image">📊</div>
                        <div class="project-content">
                            <h3 class="project-title">Data Visualization Dashboard</h3>
                            <p class="project-description">An interactive data visualization tool that processes CSV files and generates dynamic charts and insights. Built with Python and modern web frameworks, featuring real-time data processing and customizable visualization options.</p>
                            <div class="project-tech">
                                <span class="tech-tag">Python</span>
                                <span class="tech-tag">Pandas</span>
                                <span class="tech-tag">Matplotlib</span>
                                <span class="tech-tag">Flask</span>
                                <span class="tech-tag">Chart.js</span>
                            </div>
                            <div class="project-links">
                                <a href="#" class="project-link primary-link">Coming Soon</a>
                                <a href="https://github.com/BiggestZ" class="project-link secondary-link" target="_blank">GitHub</a>
                            </div>
                        </div>
                    </div>

                    <!-- Project 3 -->
                    <div class="project-card">
                        <div class="project-image">🎯</div>
                        <div class="project-content">
                            <h3 class="project-title">Task Management App</h3>
                            <p class="project-description">A full-stack task management application with user authentication, real-time updates, and collaborative features. Implements modern UI/UX principles with drag-and-drop functionality and progress tracking.</p>
                            <div class="project-tech">
                                <span class="tech-tag">React</span>
                                <span class="tech-tag">Node.js</span>
                                <span class="tech-tag">Express</span>
                                <span class="tech-tag">MongoDB</span>
                                <span class="tech-tag">Socket.io</span>
                            </div>
                            <div class="project-links">
                                <a href="#" class="project-link primary-link">In Development</a>
                                <a href="https://github.com/BiggestZ" class="project-link secondary-link" target="_blank">GitHub</a>
                            </div>
                        </div>
                    </div>

                    <!-- Project 4 -->
                    <div class="project-card">
                        <div class="project-image">🤖</div>
                        <div class="project-content">
                            <h3 class="project-title">Machine Learning Classifier</h3>
                            <p class="project-description">A machine learning project that classifies data using various algorithms. Includes data preprocessing, model training, evaluation metrics, and a web interface for predictions. Demonstrates understanding of ML concepts and implementation.</p>
                            <div class="project-tech">
                                <span class="tech-tag">Python</span>
                                <span class="tech-tag">Scikit-learn</span>
                                <span class="tech-tag">NumPy</span>
                                <span class="tech-tag">Jupyter</span>
                                <span class="tech-tag">Streamlit</span>
                            </div>
                            <div class="project-links">
                                <a href="#" class="project-link primary-link">Coming Soon</a>
                                <a href="https://github.com/BiggestZ" class="project-link secondary-link" target="_blank">GitHub</a>
                            </div>
                        </div>
                    </div>

                    <!-- Project 5 -->
                    <div class="project-card">
                        <div class="project-image">📱</div>
                        <div class="project-content">
                            <h3 class="project-title">Mobile App Prototype</h3>
                            <p class="project-description">A cross-platform mobile application prototype focusing on user experience and performance. Features include offline functionality, push notifications, and seamless navigation with modern design patterns.</p>
                            <div class="project-tech">
                                <span class="tech-tag">React Native</span>
                                <span class="tech-tag">Expo</span>
                                <span class="tech-tag">Firebase</span>
                                <span class="tech-tag">Redux</span>
                                <span class="tech-tag">TypeScript</span>
                            </div>
                            <div class="project-links">
                                <a href="#" class="project-link primary-link">In Planning</a>
                                <a href="https://github.com/BiggestZ" class="project-link secondary-link" target="_blank">GitHub</a>
                            </div>
                        </div>
                    </div>

                    <!-- Project 6 -->
                    <div class="project-card">
                        <div class="project-image">🔧</div>
                        <div class="project-content">
                            <h3 class="project-title">Developer Tools Suite</h3>
                            <p class="project-description">A collection of utility tools for developers including code formatters, API testing tools, and productivity enhancers. Built with modularity and extensibility in mind, featuring a clean command-line interface.</p>
                            <div class="project-tech">
                                <span class="tech-tag">Node.js</span>
                                <span class="tech-tag">CLI</span>
                                <span class="tech-tag">Jest</span>
                                <span class="tech-tag">ESLint</span>
                                <span class="tech-tag">npm</span>
                            </div>
                            <div class="project-links">
                                <a href="#" class="project-link primary-link">Coming Soon</a>
                                <a href="https://github.com/BiggestZ" class="project-link secondary-link" target="_blank">GitHub</a>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Coming Soon Section -->
                <div class="coming-soon">
                    <h3>More Projects Coming Soon!</h3>
                    <p>I'm constantly working on new projects and learning new technologies. Check back regularly to see my latest work, or follow me on GitHub to stay updated with my development journey.</p>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2024 Zahir Choudhry. Built with passion and code.</p>
        </div>
    </footer>

    <script>
        // Add scroll effect to header
        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            if (window.scrollY > 100) {
                header.style.background = 'rgba(255, 255, 255, 0.98)';
            } else {
                header.style.background = 'rgba(255, 255, 255, 0.95)';
            }
        });
    </script>
</body>
</html>
