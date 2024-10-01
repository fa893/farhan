<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="/nreg/assets/bootstrap/css/bootstrap.css"/>
    <link rel="stylesheet" href="/nreg/assets/css/user.css"/>
    <title>البوابة الالكترونية للطالب</title>
    <style>
        body {
            background-color: #ffffff;
        }
        #announ, .errMsg {
            display: none; /* إخفاء قسم الإعلانات والأخطاء */
        }
    </style>
    <script type="text/javascript" language="javascript" src="/nreg/js/Validate.js"></script>
    <script type="text/javascript" language="javascript" src="/nreg/js/LoginCheck.js"></script>
    <script type="text/javascript" language="javascript" src="/nreg/js/numberonly.js"></script>
    <link rel="stylesheet" type="text/css" href="/nreg/floatbox/floatbox.css">
    <script type="text/javascript" src="/nreg/floatbox/floatbox.js"></script>
</head>
<body dir="rtl">
    <div id="content" class="content container-fluid">
        <div id="header" class="hed">
            <img class="img-responsive" src="/nreg/assets/img/logo.png">
        </div>

        <section id="login" class="col-xs-12 col-sm-6 col-md-5 col-lg-4">
            <div id="loginBox" class="loginBox">
                <form method="post" id="signin" name="signin" action="/nreg/Login.do">
                    <div class="lock"><img src="assets/img/lock.png" class="fRight">
                        <p class="fRight txtLog">تسجيل الدخول</p>
                    </div>
                    <div class="fRight rowTxt">
                        <p class="labTxt fRight">الرقم الجامعي</p>
                        <input type="text" class="fRight" size="16" maxlength="10" name="UsrId" id="UsrId"
                               onKeyPress="return numberonly(this, event);" onkeyup="CheckLength(this)" value=""/>
                    </div>
                    <div class="fRight rowTxt">
                        <p class="labTxt fRight">كلمـــــــة المرور</p>
                        <input type="password" class="fRight" size=16 maxlength="100" name="password" id="password"/>
                    </div>
                    <div class="fRight rowTxt">
                        <input type="hidden" name="hash" value="UzXQnw9Ru0LzFSAF"/>
                        <button class="btn btn-success btnTxt fRight" type="submit">دخـــــــول</button>
                        <p class="fRight remTxt"><a data-toggle="modal" data-target="#largeModal" href="/nreg/restPassword.jsp">| نسيت كلمة السر؟</a></p>
                    </div>
                </form>
            </div>
        </section>

        <!-- يمكن هنا إضافة أي محتوى آخر يحتاجه الموقع -->

        <section class="foot col-lg-12 col-sm-12 col-xs-12 col-md-12">
            <p class="copRight">Copyright © 2017 - AABU Computer Center</p>
        </section>
    </div>
    <script src="assets/bootstrap/js/bootstrap.min.js"></script>
</body>
</html>
