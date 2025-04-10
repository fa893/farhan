<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="description" content="Digital Identity of Farhan Mefleh Al-Khawalda">
    <meta name="keywords" content="Farhan Mefleh Al-Khawalda, Renewable Energy, Jordan, Youth Empowerment">
    <meta name="author" content="Farhan Mefleh Al-Khawalda">
    <title>Digital Identity of Farhan Mefleh Al-Khawalda</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"></link>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');
        body {
            font-family: 'Roboto', sans-serif;
            position: relative;
            overflow: hidden;
        }
        .fade-in {
            animation: fadeIn 2s ease-in-out;
        }
        .pulse {
            animation: pulse 2s infinite;
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }
        @keyframes pulse {
            0% {
                transform: scale(1);
                box-shadow: 0 0 0 0 rgba(0, 140, 202, 0.7);
            }
            70% {
                transform: scale(1.1);
                box-shadow: 0 0 10px 10px rgba(0, 140, 202, 0);
            }
            100% {
                transform: scale(1);
                box-shadow: 0 0 0 0 rgba(0, 140, 202, 0);
            }
        }
        .background-dots {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: -1;
        }
        .dot {
            position: absolute;
            width: 8px;
            height: 8px;
            background-color: rgba(255, 255, 255, 0.5);
            border-radius: 50%;
            animation: move 10s linear infinite;
        }
        @keyframes move {
            0% {
                transform: translateY(0) translateX(0) rotate(0deg);
            }
            100% {
                transform: translateY(100vh) translateX(100vw) rotate(360deg);
            }
        }
        .section-content {
            display: none;
        }
        .section-header {
            cursor: pointer;
        }
    </style>
</head>
<body class="bg-black text-white p-5">
    <div class="background-dots">
        <div class="dot" style="top: 10%; left: 20%; animation-duration: 12s;"></div>
        <div class="dot" style="top: 30%; left: 40%; animation-duration: 15s;"></div>
        <div class="dot" style="top: 50%; left: 60%; animation-duration: 18s;"></div>
        <div class="dot" style="top: 70%; left: 80%; animation-duration: 20s;"></div>
        <div class="dot" style="top: 90%; left: 10%; animation-duration: 22s;"></div>
        <div class="dot" style="top: 20%; left: 30%; animation-duration: 25s;"></div>
        <div class="dot" style="top: 40%; left: 50%; animation-duration: 28s;"></div>
        <div class="dot" style="top: 60%; left: 70%; animation-duration: 30s;"></div>
        <div class="dot" style="top: 80%; left: 90%; animation-duration: 32s;"></div>
        <div class="dot" style="top: 10%; left: 50%; animation-duration: 35s;"></div>
        <div class="dot" style="top: 15%; left: 25%; animation-duration: 12s;"></div>
        <div class="dot" style="top: 35%; left: 45%; animation-duration: 15s;"></div>
        <div class="dot" style="top: 55%; left: 65%; animation-duration: 18s;"></div>
        <div class="dot" style="top: 75%; left: 85%; animation-duration: 20s;"></div>
        <div class="dot" style="top: 95%; left: 15%; animation-duration: 22s;"></div>
        <div class="dot" style="top: 25%; left: 35%; animation-duration: 25s;"></div>
        <div class="dot" style="top: 45%; left: 55%; animation-duration: 28s;"></div>
        <div class="dot" style="top: 65%; left: 75%; animation-duration: 30s;"></div>
        <div class="dot" style="top: 85%; left: 95%; animation-duration: 32s;"></div>
        <div class="dot" style="top: 2%; left: 42%; animation-duration: 35s;"></div>
    </div>

    <button class="theme-switch bg-blue-500 text-white py-2 px-4 rounded-full pulse" id="theme-toggle">Switch to Dark Mode</button>
    
    <h1 id="main-title" class="text-center text-4xl font-bold my-5">Digital Identity of Farhan Mefleh Al-Khawalda</h1>
    <img src="https://assets.onecompiler.app/42r523uca/42srbjrx2/3319086100.png" alt="Farhan Al-Khawalda" class="profile-image mx-auto rounded-full border-4 border-white w-36 h-36 object-cover mb-5">

    <div class="section bg-gray-800 p-5 rounded-lg mb-5 border border-white fade-in">
        <h2 class="text-2xl font-bold mb-3 section-header">About Me:</h2>
        <div class="section-content">
            <p>My name is Farhan Mefleh Al-Khawaldeh, born on February 11, 2003. I am a 21-year-old passionate about renewable energy and youth empowerment. I am a fourth-year student in Renewable and Sustainable Energy Engineering at Al al-Bayt University. I actively contribute to global sustainability initiatives and advocate for renewable energy solutions in Jordan and worldwide. My goal is to combine local expertise with global trends in sustainable development to create a positive impact.</p>
        </div>
    </div>

    <div class="section bg-gray-800 p-5 rounded-lg mb-5 border border-white fade-in">
        <h2 class="text-2xl font-bold mb-3 section-header">Personal Information:</h2>
        <div class="section-content">
            <p><strong>Full Name:</strong> Farhan Mefleh Al-Khawaldeh</p>
            <p><strong>Date of Birth:</strong> February 11, 2003</p>
            <p><strong>Nationality:</strong> Jordanian</p>
            <p><strong>Email:</strong> frhankh07@gmail.com</p>
            <p><strong>Phone (Primary):</strong> 0775573157</p>
            <p><strong>Phone (Secondary):</strong> 0781339210</p>
            <p><strong>Address:</strong> Balaama District, Mafraq Governorate, Jordan</p>
            <p><strong>National ID:</strong> 2000617154</p>
            <p><strong>Social Status:</strong> Single</p>
        </div>
    </div>

    <div class="section bg-gray-800 p-5 rounded-lg mb-5 border border-white fade-in">
        <h2 class="text-2xl font-bold mb-3 section-header">Academic Background:</h2>
        <div class="section-content">
            <p><strong>University:</strong> Al al-Bayt University</p>
            <p><strong>Major:</strong> Renewable and Sustainable Energy Engineering</p>
            <p><strong>Academic Year:</strong> Fourth Year</p>
        </div>
    </div>

    <div class="section bg-gray-800 p-5 rounded-lg mb-5 border border-white fade-in">
        <h2 class="text-2xl font-bold mb-3 section-header">Work Experience:</h2>
        <div class="section-content">
            <p><strong>Founder and General Manager:</strong> Unlimited Energy (Sep 2023 - Aug 2024)</p>
            <p><strong>Liaison Officer:</strong> Center of Excellence for Innovation and Entrepreneurship at Al al-Bayt University (Jan 2023 - Jun 2024)</p>
            <p><strong>Ambassador:</strong> E-Learning Center, Mafraq (Nov 2021 - Present)</p>
            <p><strong>Design Team Member:</strong> University News Agency (Mar 2023 - Present)</p>
            <p><strong>Volunteer:</strong> Crown Prince Foundation and "Nahno" National Platform</p>
            <p><strong>Election Monitor:</strong> Third-time monitor for 2024 elections in Jordan</p>
        </div>
    </div>

    <div class="section bg-gray-800 p-5 rounded-lg mb-5 border border-white fade-in">
        <h2 class="text-2xl font-bold mb-3 section-header">Skills and Expertise:</h2>
        <div class="section-content">
            <ul id="skills-list" class="list-disc pl-5">
                <li>Youth Leadership and Empowerment</li>
                <li>Project Management and Event Organization</li>
                <li>Graphic Design and Multimedia Editing</li>
                <li>Renewable Energy and Sustainability</li>
                <li>Global Problem-Solving and Sustainable Development</li>
                <li>Training and Facilitation</li>
            </ul>
        </div>
    </div>

    <div class="section bg-gray-800 p-5 rounded-lg mb-5 border border-white fade-in">
        <h2 class="text-2xl font-bold mb-3 section-header">Projects and Achievements:</h2>
        <div class="section-content">
            <p><strong>Shamsna JO App:</strong> Developer of the solar energy app "Shamsna JO", which provides comprehensive information about solar energy projects in Jordan, including solar panel types, angle calculations, and companies in Jordan.</p>
            <p><strong>Certificate of Appreciation:</strong> Received from "Nahno" Platform for leading a distinguished team in organizing renewable energy workshops.</p>
            <p><strong>Election Monitoring:</strong> Served as an election monitor for the 2024 elections in Jordan.</p>
        </div>
    </div>

    <div class="section bg-gray-800 p-5 rounded-lg mb-5 border border-white fade-in">
        <h2 class="text-2xl font-bold mb-3 section-header">Global Initiatives:</h2>
        <div class="section-content">
            <p>Actively involved in global sustainability efforts. Participated in multiple international conferences on renewable energy and youth empowerment, contributing to discussions on global energy challenges and solutions. I am keen on bridging local efforts with international best practices for a greener planet.</p>
        </div>
    </div>

    <div class="section bg-gray-800 p-5 rounded-lg mb-5 border border-white fade-in">
        <h2 class="text-2xl font-bold mb-3 section-header">Contact Me:</h2>
        <div class="section-content">
            <a href="mailto:frhankh07@gmail.com" class="button bg-blue-500 text-white py-2 px-4 rounded-full hover:bg-blue-700 transition duration-300">Email Me</a>
            <a href="tel:+962781339210" class="button bg-blue-500 text-white py-2 px-4 rounded-full hover:bg-blue-700 transition duration-300">Call Me</a>
            <a href="https://linkedin.com/in/farhan-mefleh-alkhawaldeh" class="button bg-blue-500 text-white py-2 px-4 rounded-full hover:bg-blue-700 transition duration-300">Connect on LinkedIn</a>
        </div>
    </div>

    <script>
        const toggleBtn = document.getElementById('theme-toggle');
        const mainTitle = document.getElementById('main-title');
        const skillsList = document.getElementById('skills-list');
        let isDarkMode = false;

        toggleBtn.addEventListener('click', function() {
            if (!isDarkMode) {
                document.body.classList.add('bg-gray-900', 'text-white');
                document.body.classList.remove('bg-black', 'text-white');
                mainTitle.classList.add('text-white');
                mainTitle.classList.remove('text-white');
                const sections = document.querySelectorAll('.section');
                sections.forEach(section => {
                    section.classList.add('bg-gray-800', 'border-white');
                    section.classList.remove('bg-gray-800', 'border-white');
                });
                const skillItems = skillsList.querySelectorAll('li');
                skillItems.forEach(item => {
                    item.classList.add('text-white');
                    item.classList.remove('text-white');
                });
                toggleBtn.textContent = 'Switch to Light Mode';
            } else {
                document.body.classList.add('bg-black', 'text-white');
                document.body.classList.remove('bg-gray-900', 'text-white');
                mainTitle.classList.add('text-white');
                mainTitle.classList.remove('text-white');
                const sections = document.querySelectorAll('.section');
                sections.forEach(section => {
                    section.classList.add('bg-gray-800', 'border-white');
                    section.classList.remove('bg-gray-800', 'border-white');
                });
                const skillItems = skillsList.querySelectorAll('li');
                skillItems.forEach(item => {
                    item.classList.add('text-white');
                    item.classList.remove('text-white');
                });
                toggleBtn.textContent = 'Switch to Dark Mode';
            }
            isDarkMode = !isDarkMode;
        });

        const sectionHeaders = document.querySelectorAll('.section-header');
        sectionHeaders.forEach(header => {
            header.addEventListener('click', () => {
                const content = header.nextElementSibling;
                content.style.display = content.style.display === 'none' ? 'block' : 'none';
            });
        });
    </script>
</body>
</html>
