<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <meta name="theme-color" content="#3498db">
    <title>Farhan Mefleh - Renewable Energy Engineer</title>
    <style>
        /* نظام الخطوط الأساسي */
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap');
        
        :root {
            --primary: #2c3e50;
            --secondary: #34495e;
            --accent: #3498db;
            --text: #2c3e50;
            --background: rgba(255, 255, 255, 0.1);
            --card-bg: rgba(255, 255, 255, 0.1);
            --shadow: 0 2px 8px rgba(0,0,0,0.1);
        }
        
        [data-theme="dark"] {
            --primary: #ecf0f1;
            --secondary: #bdc3c7;
            --text: #ecf0f1;
            --background: rgba(44, 62, 80, 0.1);
            --card-bg: rgba(52, 73, 94, 0.1);
            --shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            transition: background-color 0.3s ease, color 0.3s ease;
        }

        body {
            font-family: 'Poppins', sans-serif;
            color: var(--text);
            background: var(--background);
            line-height: 1.5;
            overflow-x: hidden;
            text-rendering: optimizeLegibility;
            -webkit-font-smoothing: antialiased;
        }

        /* تحسينات الأداء للهواتف */
        .header-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            overflow: hidden;
            background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
            will-change: transform;
        }

        /* تقليل عدد العناصر المتحركة على الهواتف */
        .animation-square {
            position: absolute;
            background: rgba(52, 152, 219, 0.15);
            animation: float 12s infinite linear;
            will-change: transform;
        }

        @keyframes float {
            0% { transform: translateY(0) rotate(0deg); opacity: 1; }
            100% { transform: translateY(-1000px) rotate(720deg); opacity: 0; }
        }

        /* تحسينات التخطيط للهواتف */
        .container {
            max-width: 100%;
            padding: 1rem;
            margin: 0 auto;
        }

        .professional-header {
            text-align: center;
            padding: 1.5rem 1rem;
            margin-bottom: 1.5rem;
            background: var(--card-bg);
            border-radius: 8px;
            box-shadow: var(--shadow);
        }

        .profile-img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid var(--card-bg);
            box-shadow: var(--shadow);
            margin-bottom: 1rem;
        }

        h1 {
            font-size: 1.6rem;
            color: var(--primary);
            margin-bottom: 0.3rem;
            font-weight: 600;
        }

        .title {
            color: var(--accent);
            font-size: 1rem;
            margin-bottom: 0.5rem;
        }

        .professional-section {
            background: var(--card-bg);
            border-radius: 8px;
            padding: 1.2rem;
            margin-bottom: 1.2rem;
            box-shadow: var(--shadow);
        }

        h2 {
            font-size: 1.2rem;
            color: var(--primary);
            margin-bottom: 0.8rem;
            position: relative;
            padding-bottom: 0.3rem;
        }

        h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 40px;
            height: 2px;
            background: var(--accent);
        }

        p, li {
            font-size: 0.9rem;
            color: var(--secondary);
            margin-bottom: 0.6rem;
        }

        ul {
            list-style-position: inside;
        }

        li {
            margin-bottom: 0.3rem;
        }

        /* تحسينات بطاقات الاتصال للهواتف */
        .contact-cards {
            display: grid;
            grid-template-columns: 1fr;
            gap: 0.8rem;
            margin-top: 1.2rem;
        }

        .contact-card {
            padding: 1rem;
            background: var(--card-bg);
            border-radius: 8px;
            box-shadow: var(--shadow);
            text-align: center;
        }

        .contact-icon {
            font-size: 1.5rem;
            color: var(--accent);
            margin-bottom: 0.5rem;
        }

        .contact-card h3 {
            font-size: 1rem;
            margin-bottom: 0.3rem;
            color: var(--primary);
        }

        .contact-card a {
            color: var(--secondary);
            text-decoration: none;
            font-size: 0.85rem;
            word-break: break-all;
        }

        /* تحسينات شريط الوقت */
        .timeline {
            position: relative;
            padding-left: 1.2rem;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 4px;
            top: 0;
            bottom: 0;
            width: 2px;
            background: var(--accent);
        }

        .timeline-item {
            position: relative;
            margin-bottom: 1.2rem;
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            left: -1.2rem;
            top: 4px;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background: var(--accent);
            border: 2px solid var(--card-bg);
        }

        .timeline-date {
            font-size: 0.8rem;
            color: var(--accent);
            margin-bottom: 0.2rem;
        }

        /* تحسينات أزرار التبديل */
        .toggle-container {
            position: fixed;
            top: 10px;
            right: 10px;
            display: flex;
            gap: 6px;
            z-index: 100;
        }

        .toggle-btn {
            width: 36px;
            height: 36px;
            border-radius: 50%;
            background: var(--card-bg);
            color: var(--text);
            border: none;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: var(--shadow);
            font-size: 1rem;
        }

        /* تحسينات التحويم للهواتف */
        @media (hover: hover) {
            .contact-card:hover, 
            .professional-section:hover,
            .professional-header:hover {
                background: white !important;
            }
            
            .contact-card:hover h3,
            .contact-card:hover a,
            .professional-section:hover h2,
            .professional-section:hover p,
            .professional-section:hover li,
            .professional-header:hover h1 {
                color: #2c3e50 !important;
            }
            
            .toggle-btn:hover {
                background: white !important;
                color: #2c3e50 !important;
            }
        }

        /* تحسينات للأجهزة الكبيرة */
        @media (min-width: 768px) {
            .container {
                max-width: 700px;
                padding: 1.5rem;
            }
            
            .professional-header {
                padding: 2rem;
            }
            
            .profile-img {
                width: 120px;
                height: 120px;
            }
            
            h1 {
                font-size: 1.8rem;
            }
            
            .contact-cards {
                grid-template-columns: repeat(2, 1fr);
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>
    <div class="toggle-container">
        <button class="toggle-btn" id="theme-toggle">
            <i class="fas fa-moon"></i>
        </button>
        <button class="toggle-btn" id="language-toggle">
            <i class="fas fa-language"></i>
        </button>
    </div>
    
    <div class="header-animation" id="animation-container"></div>
    
    <div class="container">
        <header class="professional-header">
            <img src="https://assets.onecompiler.app/42r523uca/42srbjrx2/3319086100.png" alt="Farhan Al-Khawalda" class="profile-img">
            <h1 id="name-title">Farhan Mefleh Al-Khawalda</h1>
            <p class="title" id="job-title">Renewable Energy Engineer</p>
        </header>
        
        <section class="professional-section">
            <h2 id="about-title">About Me</h2>
            <p id="about-content">I am a dedicated Renewable Energy Engineering student at Al al-Bayt University with a passion for sustainable development and youth empowerment.</p>
        </section>
        
        <section class="professional-section">
            <h2 id="experience-title">Professional Experience</h2>
            <div class="timeline">
                <div class="timeline-item">
                    <div class="timeline-date" id="exp1-date">Sep 2023 - Aug 2024</div>
                    <h3 id="exp1-title">Founder & General Manager</h3>
                    <p id="exp1-desc">Unlimited Energy - Renewable energy startup</p>
                </div>
                <div class="timeline-item">
                    <div class="timeline-date" id="exp2-date">Jan 2023 - Jun 2024</div>
                    <h3 id="exp2-title">Liaison Officer</h3>
                    <p id="exp2-desc">Center of Excellence, Al al-Bayt University</p>
                </div>
            </div>
        </section>
        
        <section class="professional-section">
            <h2 id="education-title">Education</h2>
            <p><strong id="uni-name">Al al-Bayt University</strong></p>
            <p id="degree-name">BSc in Renewable Energy Engineering</p>
            <p id="degree-status">Fourth Year Student</p>
        </section>
        
        <section class="professional-section">
            <h2 id="projects-title">Key Projects</h2>
            <ul>
                <li><strong id="project1-name">Shamsna JO App:</strong> <span id="project1-desc">Solar energy platform</span></li>
                <li><strong id="project2-name">Renewable Workshops:</strong> <span id="project2-desc">Youth training sessions</span></li>
            </ul>
        </section>
        
        <section class="professional-section">
            <h2 id="skills-title">Skills & Expertise</h2>
            <ul>
                <li id="skill1">Renewable Energy Systems</li>
                <li id="skill2">Project Management</li>
                <li id="skill3">Youth Leadership</li>
            </ul>
        </section>
        
        <section class="professional-section">
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
                    <a href="tel:+962775573157">+962 77 557 3157</a>
                </div>
                <div class="contact-card">
                    <div class="contact-icon"><i class="fab fa-linkedin"></i></div>
                    <h3 id="linkedin-label">LinkedIn</h3>
                    <a href="https://linkedin.com/in/farhan-mefleh-alkhawaldeh">farhan-mefleh-alkhawaldeh</a>
                </div>
                <div class="contact-card">
                    <div class="contact-icon"><i class="fas fa-map-marker-alt"></i></div>
                    <h3 id="address-label">Address</h3>
                    <p id="address-content">Mafraq, Jordan</p>
                </div>
            </div>
        </section>
    </div>

    <script>
        // إنشاء عناصر الرسوم المتحركة (مخفضة للهواتف)
        const animationContainer = document.getElementById('animation-container');
        const squaresCount = window.innerWidth < 768 ? 15 : 25;
        
        for (let i = 0; i < squaresCount; i++) {
            const square = document.createElement('div');
            square.classList.add('animation-square');
            
            const size = Math.random() * 40 + 15;
            const posX = Math.random() * 100;
            const posY = Math.random() * 120;
            const duration = Math.random() * 10 + 8;
            
            square.style.width = `${size}px`;
            square.style.height = `${size}px`;
            square.style.left = `${posX}%`;
            square.style.top = `${posY}%`;
            square.style.animationDuration = `${duration}s`;
            square.style.animationDelay = `${Math.random() * 5}s`;
            
            animationContainer.appendChild(square);
        }

        // تبديل الوضع الليلي
        const themeToggle = document.getElementById('theme-toggle');
        const savedTheme = localStorage.getItem('theme') || 'light';
        
        document.documentElement.setAttribute('data-theme', savedTheme);
        themeToggle.querySelector('i').className = savedTheme === 'dark' ? 'fas fa-sun' : 'fas fa-moon';
        
        themeToggle.addEventListener('click', () => {
            const currentTheme = document.documentElement.getAttribute('data-theme');
            const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
            
            document.documentElement.setAttribute('data-theme', newTheme);
            localStorage.setItem('theme', newTheme);
            themeToggle.querySelector('i').className = newTheme === 'dark' ? 'fas fa-sun' : 'fas fa-moon';
        });

        // تبديل اللغة
        const languageToggle = document.getElementById('language-toggle');
        let currentLang = 'en';
        
        const translations = {
            en: {
                name: "Farhan Mefleh Al-Khawalda",
                title: "Renewable Energy Engineer",
                aboutTitle: "About Me",
                aboutContent: "I am a dedicated Renewable Energy Engineering student at Al al-Bayt University with a passion for sustainable development and youth empowerment.",
                experienceTitle: "Professional Experience",
                exp1Date: "Sep 2023 - Aug 2024",
                exp1Title: "Founder & General Manager",
                exp1Desc: "Unlimited Energy - Renewable energy startup",
                educationTitle: "Education",
                uniName: "Al al-Bayt University",
                degreeName: "BSc in Renewable Energy Engineering",
                degreeStatus: "Fourth Year Student",
                projectsTitle: "Key Projects",
                project1Name: "Shamsna JO App:",
                project1Desc: "Solar energy platform",
                skillsTitle: "Skills & Expertise",
                skill1: "Renewable Energy Systems",
                skill2: "Project Management",
                contactTitle: "Contact Information",
                emailLabel: "Email",
                phoneLabel: "Phone",
                linkedinLabel: "LinkedIn",
                addressLabel: "Address",
                addressContent: "Mafraq, Jordan"
            },
            ar: {
                name: "فرحان مفلح الخوالدة",
                title: "مهندس طاقة متجددة",
                aboutTitle: "معلومات عني",
                aboutContent: "أنا طالب هندسة الطاقة المتجددة في جامعة آل البيت، متحمس للتنمية المستدامة وتمكين الشباب.",
                experienceTitle: "الخبرة المهنية",
                exp1Date: "سبتمبر 2023 - أغسطس 2024",
                exp1Title: "مؤسس ومدير عام",
                exp1Desc: "طاقة غير محدودة - شركة ناشئة للطاقة المتجددة",
                educationTitle: "التعليم",
                uniName: "جامعة آل البيت",
                degreeName: "بكالوريوس في هندسة الطاقة المتجددة",
                degreeStatus: "طالب في السنة الرابعة",
                projectsTitle: "المشاريع الرئيسية",
                project1Name: "تطبيق شمسنا الأردن:",
                project1Desc: "منصة للطاقة الشمسية",
                skillsTitle: "المهارات والخبرات",
                skill1: "أنظمة الطاقة المتجددة",
                skill2: "إدارة المشاريع",
                contactTitle: "معلومات الاتصال",
                emailLabel: "البريد الإلكتروني",
                phoneLabel: "الهاتف",
                linkedinLabel: "لينكدإن",
                addressLabel: "العنوان",
                addressContent: "المفرق، الأردن"
            }
        };
        
        languageToggle.addEventListener('click', () => {
            currentLang = currentLang === 'en' ? 'ar' : 'en';
            updateContent(currentLang);
            document.body.dir = currentLang === 'ar' ? 'rtl' : 'ltr';
        });
        
        function updateContent(lang) {
            const data = translations[lang];
            document.getElementById('name-title').textContent = data.name;
            document.getElementById('job-title').textContent = data.title;
            document.getElementById('about-title').textContent = data.aboutTitle;
            document.getElementById('about-content').textContent = data.aboutContent;
            document.getElementById('experience-title').textContent = data.experienceTitle;
            document.getElementById('exp1-date').textContent = data.exp1Date;
            document.getElementById('exp1-title').textContent = data.exp1Title;
            document.getElementById('exp1-desc').textContent = data.exp1Desc;
            document.getElementById('education-title').textContent = data.educationTitle;
            document.getElementById('uni-name').textContent = data.uniName;
            document.getElementById('degree-name').textContent = data.degreeName;
            document.getElementById('degree-status').textContent = data.degreeStatus;
            document.getElementById('projects-title').textContent = data.projectsTitle;
            document.getElementById('project1-name').textContent = data.project1Name;
            document.getElementById('project1-desc').textContent = data.project1Desc;
            document.getElementById('skills-title').textContent = data.skillsTitle;
            document.getElementById('skill1').textContent = data.skill1;
            document.getElementById('skill2').textContent = data.skill2;
            document.getElementById('contact-title').textContent = data.contactTitle;
            document.getElementById('email-label').textContent = data.emailLabel;
            document.getElementById('phone-label').textContent = data.phoneLabel;
            document.getElementById('linkedin-label').textContent = data.linkedinLabel;
            document.getElementById('address-label').textContent = data.addressLabel;
            document.getElementById('address-content').textContent = data.addressContent;
        }
    </script>
</body>
</html>
