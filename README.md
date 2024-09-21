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
            font-size: 32px;
            color: #007bff;
        }
        .profile-image {
            display: block;
            margin: 0 auto 20px;
            border-radius: 50%;
            width: 150px;
            height: 150px;
            object-fit: cover;
            border: 2px solid var(--text-color, #333);
            transition: transform 0.3s;
        }
        .profile-image:hover {
            transform: rotate(15deg);
        }
        .section {
            background-color: var(--section-bg-color, #f9f9f9);
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 20px;
            border: 1px solid var(--border-color, #ddd);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .button {
            display: inline-block;
            margin: 10px;
            padding: 8px 15px;
            background-color: #007bff;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-size: 14px;
            transition: background-color 0.3s, transform 0.1s;
        }
        .button:hover {
            background-color: #0056b3;
            transform: scale(1.05);
            animation: shake 0.3s;
        }
        @keyframes shake {
            0% { transform: translate(1px, 1px) rotate(0deg); }
            10% { transform: translate(-1px, -2px) rotate(-1deg); }
            20% { transform: translate(-3px, 0px) rotate(1deg); }
            30% { transform: translate(3px, 2px) rotate(0deg); }
            40% { transform: translate(1px, -1px) rotate(1deg); }
            50% { transform: translate(-1px, 2px) rotate(-1deg); }
            60% { transform: translate(-3px, 1px) rotate(0deg); }
            70% { transform: translate(3px, 1px) rotate(-1deg); }
            80% { transform: translate(-1px, -1px) rotate(1deg); }
            90% { transform: translate(1px, 2px) rotate(0deg); }
            100% { transform: translate(1px, -2px) rotate(-1deg); }
        }
        .theme-switch {
            position: absolute;
            top: 10px;
            right: 10px;
            font-size: 12px;
            padding: 5px 10px;
        }
        ul {
            list-style-type: disc;
            padding-left: 20px;
        }
    </style>
</head>
<body>

    <h1>Digital Identity of Farhan Mefleh Al-Khawalda</h1>
    <img src="https://assets.onecompiler.app/42r523uca/42srbjrx2/3319086100.png" alt="Farhan Al-Khawalda" class="profile-image">

    <button class="button theme-switch" id="theme-toggle">Switch to Dark Mode</button>

    <div class="section">
        <h2>About Me:</h2>
        <p>My name is Farhan Mefleh Al-Khawaldeh, born on February 11, 2003. I am a 21-year-old passionate about renewable energy and youth empowerment. I am a fourth-year student in Renewable and Sustainable Energy Engineering at Al al-Bayt University. I actively contribute to global sustainability initiatives and advocate for renewable energy solutions in Jordan and worldwide. My goal is to combine local expertise with global trends in sustainable development to create a positive impact.</p>
    </div>

    <!-- Additional sections remain the same -->

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
