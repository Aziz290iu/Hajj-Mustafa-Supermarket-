<!DOCTYPE html>
<html lang="fr" dir="rtl">
<head>
    <meta charset="UTF-8">
    <title></title>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            box-sizing: border-box;
            font-family: 'Cairo', sans-serif;
        }

        body {
            margin: 0;
            padding: 0;
            background-color: #ffffff; /* تعيين الخلفية إلى اللون الأبيض */
            max-width: 1400px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
        }

        .header, .nav-bar, .products-grid, .footer {
            position: relative;
            z-index: 1;
            background-color: transparent; /* تم إزالة الخلفية الزرقاء */
        }

        .header {
            padding: 0rem;  /* المسافة حول الشعار */
            color: white;  /* لون النص داخل الشعار */
            display: flex;  /* استخدام الفليكس لترتيب العناصر */
            align-items: center;  /*<!--  --> محاذاة العناصر بشكل مركزي */
            background-image: url('https://files.fm/u/myh5945qun#/view/klipartz.com.png');  /* ضع هنا رابط صورة الغلاف */
            background-size: cover;  /* تأكد أن الصورة تغطي المساحة بالكامل */
            background-position: center;  /* تحديد مركز الصورة بحيث تكون مركزة */
            height: 250px;  /* تحديد ارتفاع الغلاف */
        }

        .logo {
            width: 150px; /* زيادة عرض الشعار */
            height: 150px; /* زيادة ارتفاع الشعار */
            margin-left: 10px;
        }

        .nav-bar {
            padding: 1rem;
        }

        .nav-link {
            color: black;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr); /* عرض منتجين في نفس السطر */
            gap: 50px;
            padding: 20px;
        }

        .product-card {
            background: white(142, 68, 173, 0.06); /* اللون البنفسجي مع شفافية 60% */
            border-radius: 10px;
            padding: 15px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
        }

        .product-image {
            max-width: 100%;
            height: 200px;
            object-fit: contain;
        }

        .price {
            color: #d32f2f;
            font-weight: bold;
            font-size: 1.2em;
        }

        .footer {
            background-color: #800080;
            color: white;
            text-align: center;
            padding: 1rem;
            margin-top: 2rem;
        }

        .contact-info {
            direction: ltr;
            unicode-bidi: bidi-override;
        }
    </style>
</head>
<body>

    <header class="header">
        <img src="https://i.ibb.co/Z4nWJZL/20250408-193213.png" alt="شعار المتجر" class="logo">
        <h1></h1>
    </header>

    <nav class="nav-bar">
        <a href="#" class="nav-link">الرئيسية</a>
        <a href="#" class="nav-link">العروض</a>
        <a href="categories.html" class="nav-link">الفئات</a> <!-- رابط إلى صفحة الفئات -->
        <a href="#" class="nav-link">اتصل بنا</a>
    </nav>

    <main class="products-grid">
        <div class="product-card">
            <img src="https://i.ibb.co/WN5shjCL/125.jpg" alt="حليب لُويا" class="product-image">
            <h3>حليب لُويا</h3>
            <p class="price">12 دج</p>
            <button onclick="addToCart()">إضافة إلى السلة</button>
        </div>

        <div class="product-card">
            <img src="https://i.ibb.co/PvSvC7ZS/images-1.jpg" alt="زيت زيتون" class="product-image">
            <h3>زيت زيتون</h3>
            <p class="price">45 دج</p>
            <button onclick="addToCart()">إضافة إلى السلة</button>
        </div>
        
        <div class="product-card">
            <img src="https://i.ibb.co/yFR30XSK/images-2.jpg" alt="زبدة صول" class="product-image">
            <h3>زبدة صول</h3>
            <p class="price">17 دج</p>
            <button onclick="addToCart()">إضافة إلى السلة</button>
        </div>
    </main>

    <footer class="footer">
    <p>© 2024 جميع الحقوق محفوظة</p>
    <div class="contact-info">
         0781992008 | aziznobady@gmail.com
    </div>
    <p>تم التطوير بواسطة: بلمبروك أحمد عبد العزيز</p> <!-- إضافة اسم المطور -->
</footer>
</body>
</html>
