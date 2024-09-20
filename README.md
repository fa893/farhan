<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="description" content="Digital Identity of Farhan Mefleh Al-Khawalda">
    <meta name="keywords" content="Farhan Mefleh Al-Khawalda, Renewable Energy, Jordan, Youth Empowerment">
    <meta name="author" content="Farhan Mefleh Al-Khawalda">
    <title>Digital Identity of Farhan Mefleh Al-Khawalda</title>
    <style>
        body {
            background-color: var(--bg-color, #ffffff);
            color: var(--text-color, #333);
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 20px;
            line-height: 1.6;
        }
        h1 {
            text-align: center;
            font-size: 36px;
        }
        .profile-image {
            display: block;
            margin: 0 auto 20px;
            border-radius: 50%;
            width: 200px;
            height: 200px;
            object-fit: cover;
            border: 2px solid var(--text-color, #333);
        }
        .section {
            background-color: var(--section-bg-color, #f9f9f9);
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 20px;
            border: 1px solid var(--border-color, #ddd);
        }
        .button {
            display: inline-block;
            margin: 10px;
            padding: 10px 20px;
            background-color: #007bff;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .button:hover {
            background-color: #0056b3;
        }
        .theme-switch {
            position: absolute;
            top: 20px;
            right: 20px;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>

    <h1>Digital Identity of Farhan Mefleh Al-Khawalda</h1>
    <img src="https://assets.onecompiler.app/42r523uca/42srbjrx2/3319086100.png" alt="Farhan Al-Khawalda" class="profile-image">

    <button class="button theme-switch" id="theme-toggle">Switch to Dark Mode</button>

    <div class="section">
        <h2>About Me:</h2>
        <p>My name is Farhan Mefleh Al-Khawaldeh, born on February 11, 2003. I am a 21-year-old passionate about renewable energy and youth empowerment...</p>
    </div>

    <div class="section">
        <h2>Personal Information:</h2>
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

    <div class="section">
        <h2>Contact Me:</h2>
        <a href="mailto:frhankh07@gmail.com" class="button">Email Me</a>
        <a href="tel:+962781339210" class="button">Call Me</a>
        <a href="https://linkedin.com/in/farhan-mefleh-alkhawaldeh" class="button">Connect on LinkedIn</a>
    </div>

    <script>
        const toggleBtn = document.getElementById('theme-toggle');
        let isDarkMode = false;

        toggleBtn.addEventListener('click', function() {
            if (!isDarkMode) {
                document.documentElement.style.setProperty('--bg-color', '#333');
                document.documentElement.style.setProperty('--text-color', '#fff');
                document.documentElement.style.setProperty('--section-bg-color', '#444');
                document.documentElement.style.setProperty('--border-color', '#555');
                toggleBtn.textContent = 'Switch to Light Mode';
            } else {
                document.documentElement.style.setProperty('--bg-color', '#fff');
                document.documentElement.style.setProperty('--text-color', '#333');
                document.documentElement.style.setProperty('--section-bg-color', '#f9f9f9');
                document.documentElement.style.setProperty('--border-color', '#ddd');
                toggleBtn.textContent = 'Switch to Dark Mode';
            }
            isDarkMode = !isDarkMode;
        });
    </script>

</body>
</html>
