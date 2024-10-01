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

        .message {
            margin-top: 20px;
            padding: 10px;
            background-color: #fff3cd; /* لون خلفية الرسالة */
            color: #856404; /* لون النص */
            border: 1px solid #ffeeba; /* لون الحدود */
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="form-container">
        <form id="customForm">
            <label for="UsrId">الرقم الجامعي:</label>
            <input type="text" id="UsrId" name="UsrId" required>

            <label for="password">كلمة المرور:</label>
            <input type="password" id="password" name="password" required>

            <button type="submit">دخول</button>
        </form>
        <p>تمت محاكاة هذه البوابة من قبل المهندس فرحان الخوالده</p>
        <div id="messageContainer" class="message" style="display: none;"></div>
    </div>

    <script>
        document.getElementById("customForm").addEventListener("submit", function(event) {
            event.preventDefault(); // منع الإرسال الافتراضي للنموذج

            // الحصول على البيانات من الحقول
            var userId = document.getElementById("UsrId").value;
            var password = document.getElementById("password").value;

            // هنا يمكنك إضافة التحقق من البيانات إذا لزم الأمر
            // ...

            // عرض رسالة تطلب من المستخدم مراجعة مكتب خدمة العلم
            var messageContainer = document.getElementById("messageContainer");
            messageContainer.innerHTML = "يرجى مراجعة مكتب خدمة العلم لغايات التأجيل حيث لن تتمكن من التسجيل الا بعد مراجعة مكتب خدمة العلم في جامعة آل البيت.";
            messageContainer.style.display = "block"; // إظهار الرسالة
        });
    </script>
</body>
</html>
