# saurabh_rathva
rathva saurabh 
<!DOCTYPE html>
<html lang="gu">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>સૌરભ રાઠવા | Personal Website</title>

  <meta name="description"
        content="સૌરભ રાઠવાની વ્યક્તિગત વેબસાઇટ - ઓળખ, અભ્યાસ અને ડૉક્ટર બનવાનું લક્ષ્ય.">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, "Noto Sans Gujarati", sans-serif;
      background: #f5f7ff;
      color: #172033;
      line-height: 1.7;
    }

    /* ================= NAVBAR ================= */

    nav {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
      background: rgba(255,255,255,0.94);
      backdrop-filter: blur(12px);
      box-shadow: 0 3px 20px rgba(0,0,0,0.08);
    }

    .nav-container {
      max-width: 1150px;
      margin: auto;
      padding: 14px 25px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 24px;
      font-weight: bold;
      color: #2563eb;
      text-decoration: none;
    }

    .menu {
      display: flex;
      gap: 22px;
      list-style: none;
    }

    .menu a {
      text-decoration: none;
      color: #172033;
      font-weight: 600;
      transition: 0.3s;
    }

    .menu a:hover {
      color: #2563eb;
    }

    /* ================= HERO ================= */

    .hero {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 130px 20px 70px;

      background:
        radial-gradient(circle at top left, #dbeafe, transparent 35%),
        radial-gradient(circle at bottom right, #e0e7ff, transparent 35%),
        #f8fafc;
    }

    .hero-content {
      max-width: 850px;
      animation: fadeUp 1s ease;
    }

    .profile-circle {
      width: 155px;
      height: 155px;
      margin: 0 auto 25px;

      border-radius: 50%;

      background:
        linear-gradient(135deg, #2563eb, #7c3aed);

      display: flex;
      align-items: center;
      justify-content: center;

      color: white;
      font-size: 65px;
      font-weight: bold;

      box-shadow:
        0 15px 45px rgba(37,99,235,0.30);
    }

    .hero h1 {
      font-size: clamp(42px, 7vw, 72px);
      margin-bottom: 8px;

      background:
        linear-gradient(90deg, #2563eb, #7c3aed);

      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .hero h2 {
      font-size: 24px;
      color: #475569;
      margin-bottom: 15px;
    }

    .hero p {
      max-width: 680px;
      margin: auto;
      color: #64748b;
      font-size: 18px;
    }

    .buttons {
      margin-top: 30px;

      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
    }

    .btn {
      display: inline-block;
      padding: 13px 26px;
      border-radius: 50px;

      text-decoration: none;
      font-weight: bold;

      transition: 0.3s;
    }

    .btn-primary {
      background: #2563eb;
      color: white;

      box-shadow:
        0 8px 22px rgba(37,99,235,0.25);
    }

    .btn-primary:hover {
      transform: translateY(-3px);
      background: #1d4ed8;
    }

    .btn-outline {
      border: 2px solid #2563eb;
      color: #2563eb;
    }

    .btn-outline:hover {
      background: #2563eb;
      color: white;
    }

    /* ================= SECTION ================= */

    section {
      padding: 90px 20px;
    }

    .container {
      max-width: 1100px;
      margin: auto;
    }

    .section-title {
      text-align: center;
      margin-bottom: 45px;
    }

    .section-title h2 {
      font-size: 38px;
      margin-bottom: 10px;
    }

    .section-title p {
      color: #64748b;
    }

    /* ================= CARDS ================= */

    .about-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 25px;
    }

    .card {
      background: white;
      padding: 30px;

      border-radius: 20px;

      box-shadow:
        0 8px 30px rgba(15,23,42,0.08);

      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-7px);

      box-shadow:
        0 15px 35px rgba(15,23,42,0.12);
    }

    .card h3 {
      color: #2563eb;
      margin-bottom: 15px;
      font-size: 23px;
    }

    .info-list {
      list-style: none;
    }

    .info-list li {
      padding: 8px 0;
      border-bottom: 1px solid #eef2f7;
    }

    .info-list li:last-child {
      border-bottom: none;
    }

    /* ================= EDUCATION ================= */

    .education {
      background: #eef4ff;
    }

    .education-card {
      max-width: 750px;
      margin: auto;

      text-align: center;

      padding: 40px;

      background: white;

      border-radius: 25px;

      box-shadow:
        0 10px 35px rgba(37,99,235,0.10);
    }

    .education-icon {
      font-size: 55px;
      margin-bottom: 15px;
    }

    .education-card h3 {
      font-size: 30px;
      color: #2563eb;
      margin-bottom: 10px;
    }

    /* ================= SUBJECTS ================= */

    .subjects {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .subject {
      background: white;

      padding: 25px 15px;

      text-align: center;

      border-radius: 18px;

      box-shadow:
        0 7px 25px rgba(0,0,0,0.07);

      transition: 0.3s;
    }

    .subject:hover {
      transform: scale(1.04);
    }

    .subject span {
      font-size: 35px;
      display: block;
      margin-bottom: 10px;
    }

    .subject h3 {
      color: #334155;
    }

    /* ================= SCHOOL ================= */

    .school-section {
      background: white;
    }

    .school-card {
      text-align: center;

      max-width: 800px;

      margin: auto;

      padding: 45px 30px;

      border-radius: 25px;

      background:
        linear-gradient(
          135deg,
          #eff6ff,
          #f5f3ff
        );

      box-shadow:
        0 10px 35px rgba(0,0,0,0.07);
    }

    .school-icon {
      font-size: 65px;
      margin-bottom: 15px;
    }

    .school-card h3 {
      font-size: 28px;
      color: #2563eb;
      margin-bottom: 12px;
    }

    /* ================= DREAM ================= */

    .dream-section {
      background: #f8fafc;
    }

    .dream-card {
      max-width: 850px;

      margin: auto;

      text-align: center;

      padding: 50px 30px;

      border-radius: 30px;

      color: white;

      background:
        linear-gradient(
          135deg,
          #2563eb,
          #7c3aed
        );

      box-shadow:
        0 20px 45px rgba(37,99,235,0.22);
    }

    .doctor-icon {
      font-size: 75px;
      margin-bottom: 10px;
    }

    .dream-card h2 {
      font-size: 38px;
      margin-bottom: 12px;
    }

    .dream-card p {
      max-width: 650px;
      margin: auto;

      color: #e0e7ff;

      font-size: 18px;
    }

    .dream-card .goal {
      margin-top: 25px;

      display: inline-block;

      padding: 10px 22px;

      border-radius: 50px;

      background: rgba(255,255,255,0.15);

      border: 1px solid rgba(255,255,255,0.35);

      font-weight: bold;
    }

    /* ================= VILLAGE ================= */

    .village-box {
      text-align: center;

      background:
        linear-gradient(
          135deg,
          #2563eb,
          #7c3aed
        );

      color: white;

      border-radius: 25px;

      padding: 45px 25px;

      box-shadow:
        0 15px 40px rgba(37,99,235,0.20);
    }

    .village-box h2 {
      font-size: 35px;
      margin-bottom: 20px;
    }

    .location {
      font-size: 19px;
      line-height: 2;
    }

    /* ================= CONTACT ================= */

    .contact-card {
      max-width: 700px;

      margin: auto;

      text-align: center;

      background: white;

      padding: 40px;

      border-radius: 25px;

      box-shadow:
        0 10px 35px rgba(0,0,0,0.08);
    }

    .contact-card h2 {
      color: #2563eb;
      margin-bottom: 8px;
    }

    .contact-card p {
      color: #64748b;
      margin-bottom: 25px;
    }

    /* ================= FOOTER ================= */

    footer {
      background: #111827;

      color: white;

      text-align: center;

      padding: 35px 20px;
    }

    footer h3 {
      font-size: 22px;
      margin-bottom: 5px;
    }

    footer p {
      color: #cbd5e1;
    }

    /* ================= ANIMATION ================= */

    @keyframes fadeUp {

      from {
        opacity: 0;
        transform: translateY(30px);
      }

      to {
        opacity: 1;
        transform: translateY(0);
      }

    }

    /* ================= MOBILE ================= */

    @media (max-width: 800px) {

      .about-grid {
        grid-template-columns: 1fr;
      }

      .subjects {
        grid-template-columns: repeat(2, 1fr);
      }

      .menu {
        gap: 10px;
      }

      .menu a {
        font-size: 13px;
      }

      .section-title h2 {
        font-size: 30px;
      }

    }

    @media (max-width: 520px) {

      .nav-container {
        padding: 12px 12px;
      }

      .logo {
        font-size: 19px;
      }

      .menu {
        gap: 6px;
      }

      .menu a {
        font-size: 10px;
      }

      .hero h2 {
        font-size: 19px;
      }

      .hero p {
        font-size: 16px;
      }

      .subjects {
        grid-template-columns: 1fr 1fr;
      }

      .dream-card h2 {
        font-size: 29px;
      }

      section {
        padding: 65px 15px;
      }

    }

  </style>
</head>


<body>


  <!-- ================= NAVIGATION ================= -->

  <nav>

    <div class="nav-container">

      <a href="#home" class="logo">
        Saurabh
      </a>

      <ul class="menu">

        <li>
          <a href="#home">Home</a>
        </li>

        <li>
          <a href="#about">About</a>
        </li>

        <li>
          <a href="#education">Education</a>
        </li>

        <li>
          <a href="#school">School</a>
        </li>

        <li>
          <a href="#dream">Dream</a>
        </li>

        <li>
          <a href="#village">Village</a>
        </li>

        <li>
          <a href="#contact">Contact</a>
        </li>

      </ul>

    </div>

  </nav>


  <!-- ================= HOME ================= -->

  <section class="hero" id="home">

    <div class="hero-content">

      <div class="profile-circle">
        S
      </div>

      <h1>
        સૌરભ રાઠવા
      </h1>

      <h2>
        Student • Learner • Future Doctor 🩺
      </h2>

      <p>
        નમસ્તે! 🙏 મારું નામ સૌરભ છે.
        આ મારી વ્યક્તિગત વેબસાઇટ છે.
        અહીં તમે મારી ઓળખ, અભ્યાસ,
        શાળા અને મારા ભવિષ્યના સપના વિશે જાણી શકો છો.
      </p>

      <div class="buttons">

        <a href="#about"
           class="btn btn-primary">
          👤 મારી ઓળખ
        </a>

        <a href="#dream"
           class="btn btn-outline">
          🩺 મારું સપનું
        </a>

      </div>

    </div>

  </section>


  <!-- ================= ABOUT ================= -->

  <section id="about">

    <div class="container">

      <div class="section-title">

        <h2>
          👤 મારી ઓળખ
        </h2>

        <p>
          મારા વિશે થોડી માહિતી
        </p>

      </div>


      <div class="about-grid">


        <div class="card">

          <h3>
            🙏 મારા વિશે
          </h3>

          <p>
            મારું નામ <b>સૌરભ</b> છે.
            મારા પિતાનું નામ <b>સંજયભાઈ</b> છે.
            હું વાઘવા ગામનો રહેવાસી છું અને હાલમાં
            ધોરણ 10માં અભ્યાસ કરું છું.
          </p>

          <br>

          <p>
            મને નવી વસ્તુઓ શીખવી અને
            મારા ભવિષ્ય માટે મહેનત કરવી ગમે છે.
          </p>

        </div>


        <div class="card">

          <h3>
            📋 વ્યક્તિગત માહિતી
          </h3>

          <ul class="info-list">

            <li>
              <b>નામ:</b> સૌરભ
            </li>

            <li>
              <b>પિતાનું નામ:</b> સંજયભાઈ
            </li>

            <li>
              <b>ધોરણ:</b> 10
            </li>

            <li>
              <b>ગામ:</b> વાઘવા
            </li>

            <li>
              <b>તાલુકો:</b> બોડેલી
            </li>

            <li>
              <b>જિલ્લો:</b> છોટા ઉદેપુર
            </li>

            <li>
              <b>રાજ્ય:</b> ગુજરાત
            </li>

          </ul>

        </div>

      </div>

    </div>

  </section>


  <!-- ================= EDUCATION ================= -->

  <section class="education" id="education">

    <div class="container">

      <div class="section-title">

        <h2>
          🎓 મારો અભ્યાસ
        </h2>

        <p>
          શિક્ષણ એ સફળતાની પહેલી સીડી છે.
        </p>

      </div>


      <div class="education-card">

        <div class="education-icon">
          📚
        </div>

        <h3>
          ધોરણ 10
        </h3>

        <p>
          હું હાલમાં ધોરણ 10માં અભ્યાસ કરું છું.
          હું સારો અભ્યાસ કરીને મારા ભવિષ્યના
          લક્ષ્યને પ્રાપ્ત કરવા માગું છું.
        </p>

      </div>


      <br><br>


      <div class="section-title">

        <h2>
          📖 મારા વિષયો
        </h2>

      </div>


      <div class="subjects">

        <div class="subject">

          <span>🔬</span>

          <h3>
            Science
          </h3>

        </div>


        <div class="subject">

          <span>📐</span>

          <h3>
            Mathematics
          </h3>

        </div>


        <div class="subject">

          <span>📖</span>

          <h3>
            English
          </h3>

        </div>


        <div class="subject">

          <span>💻</span>

          <h3>
            Computer
          </h3>

        </div>

      </div>

    </div>

  </section>


  <!-- ================= SCHOOL ================= -->

  <section class="school-section" id="school">

    <div class="container">

      <div class="section-title">

        <h2>
          🏫 મારી શાળા
        </h2>

        <p>
          મારા શિક્ષણનું સ્થાન
        </p>

      </div>


      <div class="school-card">

        <div class="school-icon">
          🏫
        </div>

        <h3>
          શ્રી આદિવાસી માધ્યમિક ઉમા શાળા
        </h3>

        <p>
          હું હાલમાં ધોરણ 10માં
          <b>શ્રી આદિવાસી માધ્યમિક ઉમા શાળા</b>
          માં અભ્યાસ કરું છું.
        </p>

      </div>

    </div>

  </section>


  <!-- ================= DREAM ================= -->

  <section class="dream-section" id="dream">

    <div class="container">

      <div class="section-title">

        <h2>
          🌟 મારું ભવિષ્યનું લક્ષ્ય
        </h2>

        <p>
          મારા સપના તરફનું મારું પહેલું પગલું
        </p>

      </div>


      <div class="dream-card">

        <div class="doctor-icon">
          🩺
        </div>

        <h2>
          મારે ડૉક્ટર બનવું છે
        </h2>

        <p>
          મારું સપનું ભવિષ્યમાં ડૉક્ટર બનવાનું છે.
          હું સારો અભ્યાસ કરીને, મહેનત કરીને
          અને મારા જ્ઞાનનો ઉપયોગ કરીને લોકોની
          સેવા કરવા માગું છું.
        </p>

        <div class="goal">
          🎯 Goal: Doctor
        </div>

      </div>

    </div>

  </section>


  <!-- ================= VILLAGE ================= -->

  <section id="village">

    <div class="container">

      <div class="section-title">

        <h2>
          📍 મારું ગામ
        </h2>

        <p>
          મારા વિસ્તાર વિશે માહિતી
        </p>

      </div>


      <div class="village-box">

        <h2>
          વાઘવા ગામ 🌿
        </h2>

        <div class="location">

          📍 <b>ગામ:</b> વાઘવા
          <br>

          🏘️ <b>તાલુકો:</b> બોડેલી
          <br>

          🗺️ <b>જિલ્લો:</b> છોટા ઉદેપુર
          <br>

          🌎 <b>રાજ્ય:</b> ગુજરાત
          <br>

          🇮🇳 <b>દેશ:</b> ભારત

        </div>

      </div>

    </div>

  </section>


  <!-- ================= CONTACT ================= -->

  <section id="contact">

    <div class="container">

      <div class="section-title">

        <h2>
          📞 સંપર્ક
        </h2>

        <p>
          મારી સાથે સંપર્ક કરવા માટે
        </p>

      </div>


      <div class="contact-card">

        <h2>
          સૌરભ રાઠવા
        </h2>

        <p>
          Personal Website
        </p>

        <!--
          સુરક્ષા માટે મોબાઇલ નંબર અહીં
          સીધો જાહેર કરવામાં આવ્યો નથી.
        -->

        <a href="#"
           class="btn btn-primary"
           onclick="showContact(); return false;">
          📱 Contact Me
        </a>

        <p id="contactMessage"
           style="margin-top:20px;font-weight:bold;">
        </p>

      </div>

    </div>

  </section>


  <!-- ================= FOOTER ================= -->

  <footer>

    <h3>
      સૌરભ રાઠવા
    </h3>

    <p>
      Student • Future Doctor 🩺
    </p>

    <p>
      © 2026 Saurabh Rathva | My Personal Website
    </p>

  </footer>


  <!-- ================= JAVASCRIPT ================= -->

  <script>

    function showContact() {

      document.getElementById("contactMessage").innerHTML =
        "📞 સંપર્ક માટે તમારો મોબાઇલ નંબર અહીં ઉમેરો.";

    }

  </script>


</body>
</html>
