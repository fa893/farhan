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
            --card-bg: white;
            --header-bg: white;
            --shadow: 0 5px 15px rgba(0,0,0,0.05);
            --section-border: 4px solid var(--accent);
        }
        
        /* Dark mode variables */
        [data-theme="dark"] {
            --primary: #ecf0f1;
            --secondary: #bdc3c7;
            --accent: #3498db;
            --dark: #2c3e50;
            --light: #34495e;
            --text: #ecf0f1;
            --background: #2c3e50;
            --card-bg: #34495e;
            --header-bg: #34495e;
            --shadow: 0 5px 15px rgba(0,0,0,0.2);
            --section-border: 4px solid var(--accent);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            transition: background-color 0.3s ease, color 0.3s ease;
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
        
        /* Theme and Language Toggle */
        .toggle-container {
            position: fixed;
            top: 20px;
            right: 20px;
            display: flex;
            gap: 10px;
            z-index: 1000;
        }
        
        .toggle-btn {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: var(--card-bg);
            color: var(--text);
            border: none;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: var(--shadow);
            transition: transform 0.3s ease;
        }
        
        .toggle-btn:hover {
            transform: scale(1.1);
        }
        
        .toggle-btn i {
            font-size: 1.2rem;
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
            background: var(--header-bg);
            border-radius: 8px;
            box-shadow: var(--shadow);
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
            border: 5px solid var(--card-bg);
            box-shadow: var(--shadow);
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
            background: var(--card-bg);
            border-radius: 8px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: var(--shadow);
            border-left: var(--section-border);
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
            background: var(--card-bg);
            border-radius: 8px;
            padding: 1.5rem;
            box-shadow: var(--shadow);
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
            border: 2px solid var(--card-bg);
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
            
            .toggle-container {
                top: 10px;
                right: 10px;
            }
            
            .toggle-btn {
                width: 35px;
                height: 35px;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <!-- Theme and Language Toggle -->
    <div class="toggle-container">
        <button class="toggle-btn" id="theme-toggle" aria-label="Toggle dark mode">
            <i class="fas fa-moon"></i>
        </button>
        <button class="toggle-btn" id="language-toggle" aria-label="Toggle language">
            <i class="fas fa-language"></i>
        </button>
    </div>
    
    <!-- Professional Background Animation -->
    <div class="header-animation" id="animation-container"></div>
    
    <!-- Main Content -->
    <div class="container">
        <header class="professional-header">
            <img src="https://assets.onecompiler.app/42r523uca/42srbjrx2/3319086100.png" alt="Farhan Al-Khawalda" class="profile-img">
            <h1 id="name-title">Farhan Mefleh Al-Khawalda</h1>
            <p class="title" id="job-title">Renewable Energy Engineer</p>
        </header>
        
        <!-- About Section -->
        <section class="professional-section" style="animation-delay: 0.1s">
            <h2 id="about-title">About Me</h2>
            <p id="about-content">I am a dedicated Renewable Energy Engineering student at Al al-Bayt University with a passion for sustainable development and youth empowerment. My goal is to bridge the gap between academic knowledge and practical implementation in the renewable energy sector.</p>
        </section>
        
        <!-- Experience Section -->
        <section class="professional-section" style="animation-delay: 0.2s">
            <h2 id="experience-title">Professional Experience</h2>
            <div class="timeline">
                <div class="timeline-item">
                    <div class="timeline-date" id="exp1-date">Sep 2023 - Aug 2024</div>
                    <h3 id="exp1-title">Founder & General Manager</h3>
                    <p id="exp1-desc">Unlimited Energy - Renewable energy startup focusing on innovative solutions</p>
                </div>
                <div class="timeline-item">
                    <div class="timeline-date" id="exp2-date">Jan 2023 - Jun 2024</div>
                    <h3 id="exp2-title">Liaison Officer</h3>
                    <p id="exp2-desc">Center of Excellence for Innovation and Entrepreneurship, Al al-Bayt University</p>
                </div>
                <div class="timeline-item">
                    <div class="timeline-date" id="exp3-date">Nov 2021 - Present</div>
                    <h3 id="exp3-title">Ambassador</h3>
                    <p id="exp3-desc">E-Learning Center, Mafraq</p>
                </div>
            </div>
        </section>
        
        <!-- Education Section -->
        <section class="professional-section" style="animation-delay: 0.3s">
            <h2 id="education-title">Education</h2>
            <p><strong id="uni-name">Al al-Bayt University</strong></p>
            <p id="degree-name">Bachelor's in Renewable and Sustainable Energy Engineering</p>
            <p id="degree-status">Fourth Year Student</p>
        </section>
        
        <!-- Projects Section -->
        <section class="professional-section" style="animation-delay: 0.4s">
            <h2 id="projects-title">Key Projects</h2>
            <ul>
                <li><strong id="project1-name">Shamsna JO App:</strong> <span id="project1-desc">Comprehensive solar energy information platform for Jordan</span></li>
                <li><strong id="project2-name">Renewable Energy Workshops:</strong> <span id="project2-desc">Organized training sessions for youth</span></li>
                <li><strong id="project3-name">Election Monitoring:</strong> <span id="project3-desc">Participated as monitor in 2024 Jordan elections</span></li>
            </ul>
        </section>
        
        <!-- Skills Section -->
        <section class="professional-section" style="animation-delay: 0.5s">
            <h2 id="skills-title">Skills & Expertise</h2>
            <ul>
                <li id="skill1">Renewable Energy Systems</li>
                <li id="skill2">Project Management</li>
                <li id="skill3">Youth Leadership</li>
                <li id="skill4">Training & Facilitation</li>
                <li id="skill5">Sustainable Development</li>
            </ul>
        </section>
        
        <!-- Contact Section -->
        <section class="professional-section" style="animation-delay: 0.6s">
            <h2 id="contact-title">Contact Information</h2>
            <div class="contact-cards">
                <div class="contact-card">
                    <div class="contact-icon"><i class="fas fa-envelope"></i></div>
                    <h3 id="email-label">Email</h3>
                    <a href="mailto:frhankh07@gmail.com">frhankh07@gmail.com</a>
                </div>
                <div class="contact-card">
                    <div class="contact-icon"><i class="fas fa-phone"></i></div>
                    <h3 id="phone-label">Phone</h3>
                    <a href="tel:+962775573157">+962 77 557 3157</a><br>
                    <a href="tel:+962781339210">+962 78 133 9210</a>
                </div>
                <div class="contact-card">
                    <div class="contact-icon"><i class="fab fa-linkedin"></i></div>
                    <h3 id="linkedin-label">LinkedIn</h3>
                    <a href="https://linkedin.com/in/farhan-mefleh-alkhawaldeh">farhan-mefleh-alkhawaldeh</a>
                </div>
                <div class="contact-card">
                    <div class="contact-icon"><i class="fas fa-map-marker-alt"></i></div>
                    <h3 id="address-label">Address</h3>
                    <p id="address-content">Balaama District, Mafraq Governorate, Jordan</p>
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
        
        // Dark Mode Toggle
        const themeToggle = document.getElementById('theme-toggle');
        const themeIcon = themeToggle.querySelector('i');
        
        // Check for saved theme preference or use preferred color scheme
        const savedTheme = localStorage.getItem('theme') || 
                         (window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light');
        
        // Apply the saved theme
        document.documentElement.setAttribute('data-theme', savedTheme);
        updateThemeIcon(savedTheme);
        
        themeToggle.addEventListener('click', () => {
            const currentTheme = document.documentElement.getAttribute('data-theme');
            const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
            
            document.documentElement.setAttribute('data-theme', newTheme);
            localStorage.setItem('theme', newTheme);
            updateThemeIcon(newTheme);
        });
        
        function updateThemeIcon(theme) {
            if (theme === 'dark') {
                themeIcon.classList.remove('fa-moon');
                themeIcon.classList.add('fa-sun');
            } else {
                themeIcon.classList.remove('fa-sun');
                themeIcon.classList.add('fa-moon');
            }
        }
        
        // Language Toggle
        const languageToggle = document.getElementById('language-toggle');
        let currentLanguage = 'en'; // Default language
        
        // Arabic translations
        const translations = {
            en: {
                name: "Farhan Mefleh Al-Khawalda",
                title: "Renewable Energy Engineer",
                aboutTitle: "About Me",
                aboutContent: "I am a dedicated Renewable Energy Engineering student at Al al-Bayt University with a passion for sustainable development and youth empowerment. My goal is to bridge the gap between academic knowledge and practical implementation in the renewable energy sector.",
                experienceTitle: "Professional Experience",
                exp1Date: "Sep 2023 - Aug 2024",
                exp1Title: "Founder & General Manager",
                exp1Desc: "Unlimited Energy - Renewable energy startup focusing on innovative solutions",
                exp2Date: "Jan 2023 - Jun 2024",
                exp2Title: "Liaison Officer",
                exp2Desc: "Center of Excellence for Innovation and Entrepreneurship, Al al-Bayt University",
                exp3Date: "Nov 2021 - Present",
                exp3Title: "Ambassador",
                exp3Desc: "E-Learning Center, Mafraq",
                educationTitle: "Education",
                uniName: "Al al-Bayt University",
                degreeName: "Bachelor's in Renewable and Sustainable Energy Engineering",
                degreeStatus: "Fourth Year Student",
                projectsTitle: "Key Projects",
                project1Name: "Shamsna JO App:",
                project1Desc: "Comprehensive solar energy information platform for Jordan",
                project2Name: "Renewable Energy Workshops:",
                project2Desc: "Organized training sessions for youth",
                project3Name: "Election Monitoring:",
                project3Desc: "Participated as monitor in 2024 Jordan elections",
                skillsTitle: "Skills & Expertise",
                skill1: "Renewable Energy Systems",
                skill2: "Project Management",
                skill3: "Youth Leadership",
                skill4: "Training & Facilitation",
                skill5: "Sustainable Development",
                contactTitle: "Contact Information",
                emailLabel: "Email",
                phoneLabel: "Phone",
                linkedinLabel: "LinkedIn",
                addressLabel: "Address",
                addressContent: "Balaama District, Mafraq Governorate, Jordan"
            },
            ar: {
                name: "فرحان مفلح الخوالدة",
                title: "مهندس طاقة متجددة",
                aboutTitle: "معلومات عني",
                aboutContent: "أنا طالب هندسة الطاقة المتجددة في جامعة آل البيت، متحمس للتنمية المستدامة وتمكين الشباب. هدفي هو سد الفجوة بين المعرفة الأكاديمية والتطبيق العملي في قطاع الطاقة المتجددة.",
                experienceTitle: "الخبرة المهنية",
                exp1Date: "سبتمبر 2023 - أغسطس 2024",
                exp1Title: "مؤسس ومدير عام",
                exp1Desc: "شركة طاقة غير محدودة - شركة ناشئة تركز على حلول الطاقة المتجددة المبتكرة",
                exp2Date: "يناير 2023 - يونيو 2024",
                exp2Title: "ضابط اتصال",
                exp2Desc: "مركز التميز للابتكار وريادة الأعمال، جامعة آل البيت",
                exp3Date: "نوفمبر 2021 - حتى الآن",
                exp3Title: "سفير",
                exp3Desc: "مركز التعلم الإلكتروني، المفرق",
                educationTitle: "التعليم",
                uniName: "جامعة آل البيت",
                degreeName: "بكالوريوس في هندسة الطاقة المتجددة والمستدامة",
                degreeStatus: "طالب في السنة الرابعة",
                projectsTitle: "المشاريع الرئيسية",
                project1Name: "تطبيق شمسنا الأردن:",
                project1Desc: "منصة شاملة لمعلومات الطاقة الشمسية في الأردن",
                project2Name: "ورش عمل الطاقة المتجددة:",
                project2Desc: "تنظيم جلسات تدريبية للشباب",
                project3Name: "مراقبة الانتخابات:",
                project3Desc: "المشاركة كمراقب في انتخابات الأردن 2024",
                skillsTitle: "المهارات والخبرات",
                skill1: "أنظمة الطاقة المتجددة",
                skill2: "إدارة المشاريع",
                skill3: "قيادة الشباب",
                skill4: "التدريب والتيسير",
                skill5: "التنمية المستدامة",
                contactTitle: "معلومات الاتصال",
                emailLabel: "البريد الإلكتروني",
                phoneLabel: "الهاتف",
                linkedinLabel: "لينكدإن",
                addressLabel: "العنوان",
                addressContent: "منطقة بلعما، محافظة المفرق، الأردن"
            }
        };
        
        languageToggle.addEventListener('click', () => {
            currentLanguage = currentLanguage === 'en' ? 'ar' : 'en';
            updateLanguage(currentLanguage);
            
            // Toggle RTL for Arabic
            if (currentLanguage === 'ar') {
                document.body.setAttribute('dir', 'rtl');
            } else {
                document.body.removeAttribute('dir');
            }
        });
        
        function updateLanguage(lang) {
            // Update all text elements with translations
            document.getElementById('name-title').textContent = translations[lang].name;
            document.getElementById('job-title').textContent = translations[lang].title;
            document.getElementById('about-title').textContent = translations[lang].aboutTitle;
            document.getElementById('about-content').textContent = translations[lang].aboutContent;
            document.getElementById('experience-title').textContent = translations[lang].experienceTitle;
            document.getElementById('exp1-date').textContent = translations[lang].exp1Date;
            document.getElementById('exp1-title').textContent = translations[lang].exp1Title;
            document.getElementById('exp1-desc').textContent = translations[lang].exp1Desc;
            document.getElementById('exp2-date').textContent = translations[lang].exp2Date;
            document.getElementById('exp2-title').textContent = translations[lang].exp2Title;
            document.getElementById('exp2-desc').textContent = translations[lang].exp2Desc;
            document.getElementById('exp3-date').textContent = translations[lang].exp3Date;
            document.getElementById('exp3-title').textContent = translations[lang].exp3Title;
            document.getElementById('exp3-desc').textContent = translations[lang].exp3Desc;
            document.getElementById('education-title').textContent = translations[lang].educationTitle;
            document.getElementById('uni-name').textContent = translations[lang].uniName;
            document.getElementById('degree-name').textContent = translations[lang].degreeName;
            document.getElementById('degree-status').textContent = translations[lang].degreeStatus;
            document.getElementById('projects-title').textContent = translations[lang].projectsTitle;
            document.getElementById('project1-name').textContent = translations[lang].project1Name;
            document.getElementById('project1-desc').textContent = translations[lang].project1Desc;
            document.getElementById('project2-name').textContent = translations[lang].project2Name;
            document.getElementById('project2-desc').textContent = translations[lang].project2Desc;
            document.getElementById('project3-name').textContent = translations[lang].project3Name;
            document.getElementById('project3-desc').textContent = translations[lang].project3Desc;
            document.getElementById('skills-title').textContent = translations[lang].skillsTitle;
            document.getElementById('skill1').textContent = translations[lang].skill1;
            document.getElementById('skill2').textContent = translations[lang].skill2;
            document.getElementById('skill3').textContent = translations[lang].skill3;
            document.getElementById('skill4').textContent = translations[lang].skill4;
            document.getElementById('skill5').textContent = translations[lang].skill5;
            document.getElementById('contact-title').textContent = translations[lang].contactTitle;
            document.getElementById('email-label').textContent = translations[lang].emailLabel;
            document.getElementById('phone-label').textContent = translations[lang].phoneLabel;
            document.getElementById('linkedin-label').textContent = translations[lang].linkedinLabel;
            document.getElementById('address-label').textContent = translations[lang].addressLabel;
            document.getElementById('address-content').textContent = translations[lang].addressContent;
        }
    </script>
</body>
</html>
