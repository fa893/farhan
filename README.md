<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>البوابة الالكترونية للطالب - محاكاة</title>
    <style>
        body {
            background-color: #008000; /* لون الخلفية الأخضر */
            color: white; /* لون النص */
            font-family: 'Arial', sans-serif;
            direction: rtl;
        }

        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .login-box {
            background-color: white; /* خلفية إدخال المعلومات */
            color: #008000;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 300px;
        }

        .login-box h2 {
            text-align: center;
            margin-bottom: 20px;
        }

        .input-group {
            margin-bottom: 15px;
        }

        .input-group label {
            display: block;
            font-weight: bold;
            margin-bottom: 5px;
        }

        .input-group input {
            width: 100%;
            padding: 10px;
            border: 1px solid #008000;
            border-radius: 5px;
            box-sizing: border-box;
        }

        .btn-submit {
            width: 100%;
            padding: 10px;
            background-color: #008000;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        .btn-submit:hover {
            background-color: #006600;
        }

        .footer {
            text-align: center;
            margin-top: 20px;
            color: white;
        }

        .footer p {
            margin: 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="login-box">
            <h2>تسجيل الدخول</h2>
            <form action="#" method="post">
                <div class="input-group">
                    <label for="student-id">الرقم الجامعي</label>
                    <input type="text" id="student-id" name="student-id" required>
                </div>
                <div class="input-group">
                    <label for="password">كلمة المرور</label>
                    <input type="password" id="password" name="password" required>
                </div>
                <button type="submit" class="btn-submit">دخول</button>
            </form>
        </div>
    </div>

    <div class="footer">
        <p>تمت محاكاة هذه البوابة من قبل المهندس فرحان الخوالده</p>
    </div>
</body>
</html>
