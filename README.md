<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"لل
    "http://www.w3.org/TR/html4/loose.dtd">
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
            .hidden {
                display: none;
            }
        </style>
    </head>
    <body dir="rtl">
        <div id="content" class="content container-fluid">
            <div id="header" class="hed"><img class="img-responsive" src="/nreg/assets/img/logo.png"></div>

            <section id="skipNotifications" class="col-xs-12 col-sm-12 col-md-12 col-lg-12">
                <button id="skipButton" class="btn btn-primary">تجاوز الإعلانات</button>
            </section>

            <section id="announ" class="announ col-lg-12 col-sm-12 col-xs-12 col-md-12 txtR hidden">
                <div class="announTxt">
                    <p><strong>الإعلانات</strong></p>
                </div>
            </section>
            <section class="announList col-lg-12 col-sm-12 col-xs-12 col-md-12 hidden">
                <div class="announLstCont">
                    <p></p>
                    <!-- يمكنك إضافة المزيد من الإعلانات هنا -->
                </div>
            </section>

            <section id="login" class="col-xs-12 col-sm-6 col-md-5 col-lg-4">
                <div id="loginBox" class="loginBox">
                    <form method="post" id="signin" name="signin" action="/nreg/Login.do">
                        <div class="lock"><img src="assets/img/lock.png" class="fRight">
                            <p class="fRight txtLog">تسجيل الدخول</p>
                        </div>
                        <div class="fRight rowTxt">
                            <p class="labTxt fRight">الرقم الجامعي</p>
                            <input type="text" class="fRight"  size="16"  maxlength="10" name="UsrId" id="UsrId"/>
                        </div>
                        <div class="fRight rowTxt">
                            <p class="labTxt fRight">كلمـــــــة المرور </p>
                            <input type="password" class="fRight" size=16 maxlength="100" name="password" id="password"/>
                        </div>
                        <div class="fRight rowTxt">
                            <button class="btn btn-success btnTxt fRight" type="submit">دخـــــــول </button>
                            <p class="fRight remTxt"><a href="/nreg/restPassword.jsp">| نسيت كلمة السر؟</a></p>
                        </div>
                    </form>
                </div>
            </section>
        </div>

        <script src="/nreg/assets/bootstrap/js/bootstrap.min.js"></script>
        <script>
            document.getElementById("skipButton").onclick = function() {
                // إخفاء قسم الإعلانات
                document.getElementById("announ").classList.add("hidden");
                document.querySelector(".announList").classList.add("hidden");
            };
        </script>
    </body>
</html>
