<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>كافينو - Cafino</title>
  <link href="https://fonts.googleapis.com/css2?family=Amiri&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Amiri', serif;
      background: linear-gradient(45deg, #ffecd2, #fcb69f, #a1c4fd);
      margin: 0;
      padding: 0;
      direction: rtl;
    }

    header {
      background-color: #6a0572;
      color: white;
      text-align: center;
      padding: 1rem 0.5rem;
      font-size: 0.9rem;
    }

    .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }

    .nav {
      display: flex;
      justify-content: space-around;
      background-color: #fff;
      padding: 0.5rem;
      flex-wrap: wrap;
      font-size: 0.9rem;
    }

    .nav a {
      padding: 0.5rem;
      text-decoration: none;
      color: #6a0572;
      font-weight: bold;
      background-color: #ffeaa7;
      border-radius: 5px;
      margin: 3px;
      cursor: pointer;
      transition: 0.2s;
    }

    .nav a:hover {
background-color: #fab1a0;
      color: #2d3436;
    }

    .content {
      max-width: 360px;
      margin: auto;
      padding: 1rem;
    }

    .section {
      display: none;
      opacity: 0;
      transform: scale(0.95);
      transition: all 0.4s ease;
    }

    .section.active {
      display: block;
      opacity: 1;
      transform: scale(1);
    }

    .post {
      background: #ffffffcc;
      padding: 0.8rem;
      margin-bottom: 1rem;
      border-radius: 10px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    footer {
      text-align: center;
      padding: 0.7rem;
      font-size: 0.8rem;
      color: #444;
    }
  </style>
</head>
<body>

  <header>
    <div class="logo">كافينو - Cafino</div>
    <p>منصتك للكورسات والمنح والمواقع المفيدة</p>
  </header>

  <div class="nav">
    <a onclick="showSection('courses')">كورسات</a>
    <a onclick="showSection('scholarships')">منح</a>
    <a onclick="showSection('tools')">مواقع</a>
  </div>

  <div class="content">
    <div id="courses" class="section">
      <div class="post">
        <h3>كورس HTML & CSS</h3>
        <p>مناسب للمبتدئين - يبدأ من الأساسيات إلى الاحتراف.</p>
      </div>
      <div class="post">
        <h3>كورس Python</h3>
        <p>أساسيات البرمجة بلغة بايثون للمبتدئين بالكامل.</p>
</div>
      <div class="post">
        <h3>كورس تصميم الجرافيك</h3>
        <p>تعلم التصميم باستخدام Photoshop و Canva.</p>
      </div>
    </div>

    <div id="scholarships" class="section">
      <div class="post">
        <h3>منحة كندا 2025</h3>
        <p>ممولة بالكامل مع راتب شهري.</p>
      </div>
      <div class="post">
        <h3>  منحة الحكومية الروسية 2025</h3>
        <p> مقاعد منحة روسيا قربت تخلص!
دي فرصتكم الأخيرة، وما تتأخّروا، لأن السنة الجاية لازم تنتظروا!

مزايا المنحة الرائعة:

دراسة في بلد متطور ومتحضر، بيئة مناسبة للجميع

أكثر من 32 جامعة حكومية للاختيار منها

دعم كل التخصصات: الأدبية، العلمية، الهندسية، وحتى الطب بكل مجالاته

مزايا شاملة: دراسة، سكن، راتب شهري ثابت، وتأمين صحي

فرص تدريب وبحث علمي مميزة

فرص عمل داخل وخارج روسيا حسب الالتزام والتفوق

 بيئة دراسية متكاملة: مراجع، معامل، وكل شيء متطور


لا تضيعوا الفرصة وابدأوا بالتقديم أو الاستفسار فوراً من هنا:
   https://grabscholarship.com
          russian-government</p>
        
     </div>
      <div class="post">
        <h3>منحة ألمانيا DAAD</h3>
        <p>تخصصات متعددة، تمويل ممتاز.</p>
      </div>
    </div>

    <div id="tools" class="section">
      <div class="post">
        <h3>موقع Remove.bg</h3>
        <p>لحذف خلفية الصور خلال ثواني مجاناً.</p>
      </div>
    </div>
  </div>

  <footer>
    &copy; 2025 - Cafino
  </footer>

  <script>
    function showSection(id) {
      document.querySelectorAll('.section').forEach(section => {
        section.classList.remove('active');
      });
      const target = document.getElementById(id);
      if (target) {
        target.classList.add('active');
      }
    }
  </script>

</body>
</html>

