<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Simulation</title>
    <style>
        body {
            background-color: #008000; /* اللون الأخضر */
            color: white; /* اللون الأبيض للنص */
        }

        .form-container {
            margin: 50px auto;
            padding: 20px;
            width: 300px;
            background-color: white;
            color: #008000; /* لون النص داخل النموذج */
            border-radius: 10px;
        }

        input[type="text"], input[type="password"] {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #008000;
            border-radius: 5px;
        }

        button {
            background-color: #008000;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: white;
            color: #008000;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <form action="https://student.aabu.edu.jo/nreg/" method="POST">
            <label for="UsrId">الرقم الجامعي:</label>
            <input type="text" id="UsrId" name="UsrId" required>

            <label for="password">كلمة المرور:</label>
            <input type="password" id="password" name="password" required>

            <button type="submit">دخول</button>
        </form>
        <p>تمت محاكاة هذه البوابة من قبل المهندس فرحان الخوالده</p>
    </div>
</body>
</html>
