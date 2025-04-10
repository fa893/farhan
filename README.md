<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Portfolio - Farhan Mefleh Al-Khawalda</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        :root {
            --primary: #2c3e50;
            --secondary: #34495e;
            --accent: #3498db;
            --dark: #2c3e50;
            --light: #ecf0f1;
            --text: #2c3e50;
            --background: #f9f9f9;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--background);
            color: var(--text);
            line-height: 1.6;
        }
        
        /* Professional Header Animation */
        .header-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            overflow: hidden;
        }
        
        .animation-square {
            position: absolute;
            background: rgba(52, 152, 219, 0.1);
            border: 1px solid rgba(52, 152, 219, 0.2);
            animation: float 15s infinite linear;
        }
        
        @keyframes float {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(-1000px) rotate(720deg);
                opacity: 0;
            }
        }
        
        /* Main Container */
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 2rem;
        }
        
        /* Professional Header */
        .professional-header {
            text-align: center;
            margin-bottom: 3rem;
            padding: 2rem 0;
            position: relative;
        }
        
        .professional-header::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: var(--accent);
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid white;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            margin-bottom: 1.5rem;
            transition: transform 0.5s ease;
        }
        
        .profile-img:hover {
            transform: scale(1.05);
        }
        
        h1 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
            font-weight: 600;
        }
        
        .title {
            color: var(--accent);
            font-weight: 400;
            margin-bottom: 1.5rem;
        }
        
        /* Professional Sections */
        .professional-section {
            background: white;
            border-radius: 8px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            border-left: 4px solid var(--accent);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 0.8s forwards;
        }
        
        .professional-section:hover {
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }
        
        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        h2 {
            font-size: 1.5rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
            position: relative;
            padding-bottom: 0.5rem;
        }
        
        h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 2px;
            background: var(--accent);
        }
        
        p, li {
            margin-bottom: 1rem;
            color: var(--secondary);
        }
        
        ul {
            list-style-position: inside;
            margin-bottom: 1.5rem;
        }
        
        li {
            margin-bottom: 0.5rem;
        }
        
        /* Contact Cards */
        .contact-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }
        
        .contact-card {
            background: white;
            border-radius: 8px;
            padding: 1.5rem;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            border-top: 3px solid var(--accent);
            transition: transform 0.3s ease;
            text-align: center;
        }
        
        .contact-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
        }
        
        .contact-icon {
            font-size: 2rem;
            color: var(--accent);
            margin-bottom: 1rem;
        }
        
        .contact-card h3 {
            color: var(--primary);
            margin-bottom: 0.5rem;
        }
        
        .contact-card a {
            color: var(--secondary);
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .contact-card a:hover {
            color: var(--accent);
        }
        
        /* Timeline for Experience */
        .timeline {
            position: relative;
            padding-left: 2rem;
        }
        
        .timeline::before {
            content: '';
            position: absolute;
            left: 7px;
            top: 0;
            bottom: 0;
            width: 2px;
            background: var(--accent);
        }
        
        .timeline-item {
            position: relative;
            margin-bottom: 2rem;
        }
        
        .timeline-item::before {
            content: '';
            position: absolute;
            left: -2rem;
            top: 5px;
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: var(--accent);
            border: 2px solid white;
        }
        
        .timeline-date {
            color: var(--accent);
            font-weight: 500;
            margin-bottom: 0.5rem;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .container {
                padding: 1.5rem;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .professional-section {
                padding: 1.5rem;
            }
            
            .contact-cards {
                grid-template-columns: 1fr;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <!-- Professional Background Animation -->
    <div class="header-animation" id="animation-container"></div>
    
    <!-- Main Content -->
    <div class="container">
        <header class="professional-header">
            <img src="https://assets.onecompiler.app/42r523uca/42srbjrx2/3319086100.png" alt="Farhan Al-Khawalda" class="profile-img">
            <h1>Farhan Mefleh Al-Khawalda</h1>
            <p class="title">Renewable Energy Engineer</p>
        </header>
        
        <!-- About Section -->
        <section class="professional-section" style="animation-delay: 0.1s">
            <h2>About Me</h2>
            <p>I am a dedicated Renewable Energy Engineering student at Al al-Bayt University with a passion for sustainable development and youth empowerment. My goal is to bridge the gap between academic knowledge and practical implementation in the renewable energy sector.</p>
        </section>
        
        <!-- Experience Section -->
        <section class="professional-section" style="animation-delay: 0.2s">
            <h2>Professional Experience</h2>
            <div class="timeline">
                <div class="timeline-item">
                    <div class="timeline-date">Sep 2023 - Aug 2024</div>
                    <h3>Founder & General Manager</h3>
                    <p>Unlimited Energy - Renewable energy startup focusing on innovative solutions</p>
                </div>
                <div class="timeline-item">
                    <div class="timeline-date">Jan 2023 - Jun 2024</div>
                    <h3>Liaison Officer</h3>
                    <p>Center of Excellence for Innovation and Entrepreneurship, Al al-Bayt University</p>
                </div>
                <div class="timeline-item">
                    <div class="timeline-date">Nov 2021 - Present</div>
                    <h3>Ambassador</h3>
                    <p>E-Learning Center, Mafraq</p>
                </div>
            </div>
        </section>
        
        <!-- Education Section -->
        <section class="professional-section" style="animation-delay: 0.3s">
            <h2>Education</h2>
            <p><strong>Al al-Bayt University</strong></p>
            <p>Bachelor's in Renewable and Sustainable Energy Engineering</p>
            <p>Fourth Year Student</p>
        </section>
        
        <!-- Projects Section -->
        <section class="professional-section" style="animation-delay: 0.4s">
            <h2>Key Projects</h2>
            <ul>
                <li><strong>Shamsna JO App:</strong> Comprehensive solar energy information platform for Jordan</li>
                <li><strong>Renewable Energy Workshops:</strong> Organized training sessions for youth</li>
                <li><strong>Election Monitoring:</strong> Participated as monitor in 2024 Jordan elections</li>
            </ul>
        </section>
        
        <!-- Skills Section -->
        <section class="professional-section" style="animation-delay: 0.5s">
            <h2>Skills & Expertise</h2>
            <ul>
                <li>Renewable Energy Systems</li>
                <li>Project Management</li>
                <li>Youth Leadership</li>
                <li>Training & Facilitation</li>
                <li>Sustainable Development</li>
            </ul>
        </section>
        
        <!-- Contact Section -->
        <section class="professional-section" style="animation-delay: 0.6s">
            <h2>Contact Information</h2>
            <div class="contact-cards">
                <div class="contact-card">
                    <div class="contact-icon"><i class="fas fa-envelope"></i></div>
                    <h3>Email</h3>
                    <a href="mailto:frhankh07@gmail.com">frhankh07@gmail.com</a>
                </div>
                <div class="contact-card">
                    <div class="contact-icon"><i class="fas fa-phone"></i></div>
                    <h3>Phone</h3>
                    <a href="tel:+962775573157">+962 77 557 3157</a><br>
                    <a href="tel:+962781339210">+962 78 133 9210</a>
                </div>
                <div class="contact-card">
                    <div class="contact-icon"><i class="fab fa-linkedin"></i></div>
                    <h3>LinkedIn</h3>
                    <a href="https://linkedin.com/in/farhan-mefleh-alkhawaldeh">farhan-mefleh-alkhawaldeh</a>
                </div>
                <div class="contact-card">
                    <div class="contact-icon"><i class="fas fa-map-marker-alt"></i></div>
                    <h3>Address</h3>
                    <p>Balaama District, Mafraq Governorate, Jordan</p>
                </div>
            </div>
        </section>
    </div>
    
    <script>
        // Create background animation elements
        const animationContainer = document.getElementById('animation-container');
        for (let i = 0; i < 15; i++) {
            const square = document.createElement('div');
            square.classList.add('animation-square');
            
            // Random properties
            const size = Math.random() * 100 + 50;
            const posX = Math.random() * 100;
            const posY = Math.random() * 100;
            const delay = Math.random() * 15;
            const duration = Math.random() * 20 + 10;
            
            square.style.width = `${size}px`;
            square.style.height = `${size}px`;
            square.style.left = `${posX}%`;
            square.style.top = `${posY}%`;
            square.style.animationDelay = `${delay}s`;
            square.style.animationDuration = `${duration}s`;
            
            animationContainer.appendChild(square);
        }
        
        // Animate sections on scroll
        const sections = document.querySelectorAll('.professional-section');
        
        function animateOnScroll() {
            sections.forEach(section => {
                const sectionTop = section.getBoundingClientRect().top;
                const windowHeight = window.innerHeight;
                
                if (sectionTop < windowHeight * 0.8) {
                    const delay = section.style.animationDelay || '0s';
                    section.style.animation = `fadeInUp 0.8s ${delay} forwards`;
                }
            });
        }
        
        // Initialize animation
        window.addEventListener('load', animateOnScroll);
        window.addEventListener('scroll', animateOnScroll);
        
        // Set initial animation delays
        let delay = 0.1;
        sections.forEach(section => {
            section.style.animationDelay = `${delay}s`;
            delay += 0.1;
        });
    </script>
</body>
</html>
