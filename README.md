<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>व्यापार सभा नोएडा महानगर</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, "Noto Sans Devanagari", sans-serif;
      color: #12304a;
      background: #f7fafc;
      line-height: 1.7;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    /* HEADER */
    header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: white;
      border-bottom: 1px solid #ddd;
      box-shadow: 0 2px 10px rgba(0,0,0,0.08);
    }

    .navbar {
      max-width: 1200px;
      margin: auto;
      padding: 14px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .logo-area h2 {
      font-size: 25px;
      color: #12304a;
    }

    .logo-area span {
      color: #e47b00;
      font-size: 14px;
    }

    nav {
      display: flex;
      gap: 22px;
      flex-wrap: wrap;
      justify-content: center;
    }

    nav a {
      font-weight: bold;
      color: #12304a;
      transition: 0.3s;
    }

    nav a:hover {
      color: #e47b00;
    }

    /* HERO */
    .hero {
      background: linear-gradient(120deg, #fff8e9, #eef8ff);
      padding: 80px 20px;
    }

    .hero-inner {
      max-width: 1100px;
      margin: auto;
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 50px;
      align-items: center;
    }

    .tag {
      display: inline-block;
      background: #fff0cf;
      color: #d66d00;
      padding: 6px 16px;
      border-radius: 30px;
      font-weight: bold;
      margin-bottom: 20px;
    }

    .hero h1 {
      font-size: 60px;
      line-height: 1.15;
      margin-bottom: 20px;
    }

    .hero h1 span {
      color: #df7600;
    }

    .hero p {
      font-size: 20px;
      margin-bottom: 25px;
      color: #4b6070;
    }

    .btn {
      display: inline-block;
      background: #e67b00;
      color: white;
      padding: 12px 25px;
      border-radius: 8px;
      font-weight: bold;
      border: none;
      cursor: pointer;
    }

    .btn:hover {
      background: #c96500;
    }

    .hero-card {
      background: white;
      padding: 35px;
      border-radius: 20px;
      box-shadow: 0 10px 35px rgba(0,0,0,0.08);
    }

    .hero-card .icon {
      font-size: 55px;
      margin-bottom: 15px;
    }

    .hero-card h2 {
      font-size: 30px;
      margin-bottom: 10px;
    }

    /* COMMON */
    section {
      padding: 70px 20px;
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
      font-size: 42px;
      color: #12304a;
    }

    .section-title p {
      color: #667784;
      font-size: 18px;
    }

    /* ABOUT */
    .about {
      background: white;
    }

    .about-box {
      background: #f5f9fc;
      padding: 35px;
      border-radius: 18px;
      text-align: center;
    }

    .about-box p {
      font-size: 19px;
      color: #526575;
    }

    /* OFFICIALS */
    .officials {
      background: #f7fafc;
    }

    .official-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 30px;
    }

    .person-card {
      background: white;
      padding: 25px;
      border-radius: 18px;
      text-align: center;
      box-shadow: 0 5px 20px rgba(0,0,0,0.06);
    }

    .person-card img {
      width: 180px;
      height: 180px;
      object-fit: cover;
      border-radius: 50%;
      border: 5px solid #e67b00;
      margin-bottom: 15px;
    }

    .person-card h3 {
      font-size: 26px;
      margin-bottom: 5px;
    }

    .person-card p {
      color: #e67b00;
      font-weight: bold;
    }

    /* EVENTS */
    .events {
      background: white;
    }

    .event-box {
      padding: 30px;
      border-left: 6px solid #e67b00;
      background: #fff8ed;
      border-radius: 10px;
      margin-bottom: 20px;
    }

    .event-box h3 {
      font-size: 25px;
      margin-bottom: 8px;
    }

    /* GALLERY */
    .gallery {
      background: #f2f7fa;
    }

    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 20px;
    }

    .gallery-item {
      background: white;
      padding: 10px;
      border-radius: 15px;
      box-shadow: 0 5px 18px rgba(0,0,0,0.08);
      overflow: hidden;
    }

    .gallery-item img {
      width: 100%;
      height: 230px;
      object-fit: cover;
      display: block;
      border-radius: 10px;
      cursor: pointer;
      transition: transform 0.3s;
    }

    .gallery-item img:hover {
      transform: scale(1.04);
    }

    .gallery-item p {
      text-align: center;
      padding: 10px 5px 5px;
      font-weight: bold;
    }

    /* MEMBERSHIP */
    .membership {
      background: white;
    }

    .form-box {
      max-width: 800px;
      margin: auto;
      background: #f6f9fb;
      padding: 35px;
      border-radius: 18px;
    }

    .form-row {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
    }

    label {
      display: block;
      margin-bottom: 6px;
      font-weight: bold;
    }

    input,
    textarea {
      width: 100%;
      padding: 13px;
      border: 1px solid #ccd6dd;
      border-radius: 8px;
      margin-bottom: 18px;
      font-size: 16px;
    }

    textarea {
      min-height: 120px;
      resize: vertical;
    }

    /* CONTACT */
    .contact {
      background: #12304a;
      color: white;
      text-align: center;
    }

    .contact h2 {
      font-size: 38px;
      margin-bottom: 15px;
    }

    .contact p {
      font-size: 18px;
      margin-bottom: 8px;
    }

    /* FOOTER */
    footer {
      background: #0b2235;
      color: white;
      text-align: center;
      padding: 22px;
    }

    /* MOBILE */
    @media (max-width: 850px) {

      .navbar {
        flex-direction: column;
      }

      nav {
        gap: 12px;
      }

      .hero-inner {
        grid-template-columns: 1fr;
      }

      .hero h1 {
        font-size: 42px;
      }

      .gallery-grid {
        grid-template-columns: repeat(2, 1fr);
      }

      .official-grid {
        grid-template-columns: 1fr;
      }
    }

    @media (max-width: 550px) {

      .gallery-grid {
        grid-template-columns: 1fr;
      }

      .form-row {
        grid-template-columns: 1fr;
      }

      .hero h1 {
        font-size: 35px;
      }

      nav {
        font-size: 14px;
      }
    }
  </style>
</head>

<body>

  <!-- HEADER -->
  <header>
    <div class="navbar">

      <div class="logo-area">
        <h2>व्यापार सभा</h2>
        <span>नोएडा महानगर</span>
      </div>

      <nav>
        <a href="#about">हमारे बारे में</a>
        <a href="#officials">पदाधिकारी</a>
        <a href="#events">कार्यक्रम</a>
        <a href="#gallery">गैलरी</a>
        <a href="#membership">सदस्यता</a>
        <a href="#contact">संपर्क</a>
      </nav>

    </div>
  </header>


  <!-- HERO -->
  <section class="hero">

    <div class="hero-inner">

      <div>

        <div class="tag">🤝 एकता • सहयोग • विकास</div>

        <h1>
          व्यापार सभा<br>
          <span>नोएडा महानगर</span>
        </h1>

        <p>
          नोएडा के व्यापारियों को एक मंच पर जोड़ने और
          व्यापारिक समुदाय के विकास के लिए समर्पित।
        </p>

        <a href="#membership" class="btn">
          सदस्य बनें
        </a>

      </div>

      <div class="hero-card">

        <div class="icon">🏪</div>

        <h2>
          मजबूत व्यापारी,<br>
          मजबूत बाजार
        </h2>

        <p>
          संवाद, सहयोग और सामूहिक पहल।
        </p>

      </div>

    </div>

  </section>


  <!-- ABOUT -->
  <section class="about" id="about">

    <div class="container">

      <div class="section-title">
        <h2>हमारे बारे में</h2>
        <p>व्यापारियों की एकता और विकास के लिए एक मंच</p>
      </div>

      <div class="about-box">

        <p>
          व्यापार सभा नोएडा महानगर का उद्देश्य नोएडा के
          व्यापारियों को एकजुट करना, उनकी समस्याओं को
          उचित मंच तक पहुंचाना तथा व्यापारिक समुदाय के
          विकास में सहयोग करना है।
        </p>

        <br>

        <p>
          हमारा प्रयास है कि सभी व्यापारी आपसी सहयोग,
          सम्मान और एकता के साथ आगे बढ़ें।
        </p>

      </div>

    </div>

  </section>


  <!-- OFFICIALS -->
  <section class="officials" id="officials">

    <div class="container">

      <div class="section-title">
        <h2>पदाधिकारी</h2>
        <p>व्यापार सभा नोएडा महानगर</p>
      </div>

      <div class="official-grid">

        <div class="person-card">

          <img src="president.jpg" alt="अध्यक्ष">

          <h3>अध्यक्ष</h3>

          <p>
            व्यापार सभा नोएडा महानगर
          </p>

        </div>


        <div class="person-card">

          <img src="secretary.jpg" alt="महासचिव">

          <h3>शिवकुमार यादव</h3>

          <p>
            महासचिव, व्यापार सभा
          </p>

        </div>

      </div>

    </div>

  </section>


  <!-- EVENTS -->
  <section class="events" id="events">

    <div class="container">

      <div class="section-title">
        <h2>कार्यक्रम</h2>
        <p>हमारी गतिविधियां और आगामी कार्यक्रम</p>
      </div>

      <div class="event-box">

        <h3>🤝 व्यापारियों की बैठक</h3>

        <p>
          व्यापारियों की समस्याओं, सुझावों और
          संगठन की आगामी योजनाओं पर चर्चा।
        </p>

      </div>

      <div class="event-box">

        <h3>📢 व्यापारी संवाद</h3>

        <p>
          व्यापारिक समुदाय के साथ संवाद और
          सहयोग को मजबूत करने की पहल।
        </p>

      </div>

    </div>

  </section>


  <!-- GALLERY -->
  <section class="gallery" id="gallery">

    <div class="container">

      <div class="section-title">

        <h2>फोटो गैलरी</h2>

        <p>
          हमारी गतिविधियों और यादगार पलों की झलक
        </p>

      </div>


      <div class="gallery-grid">

        <!-- PHOTO 1 -->
        <div class="gallery-item">

          <img
            src="photo1.jpg"
            alt="व्यापार सभा कार्यक्रम फोटो 1"
            loading="lazy"
          >

          <p>हमारी झलक - फोटो 1</p>

        </div>


        <!-- PHOTO 2 -->
        <div class="gallery-item">

          <img
            src="photo2.jpg"
            alt="व्यापार सभा कार्यक्रम फोटो 2"
            loading="lazy"
          >

          <p>हमारी झलक - फोटो 2</p>

        </div>


        <!-- PHOTO 3 -->
        <div class="gallery-item">

          <img
            src="photo3.jpg"
            alt="व्यापार सभा कार्यक्रम फोटो 3"
            loading="lazy"
          >

          <p>हमारी झलक - फोटो 3</p>

        </div>


        <!-- PHOTO 4 -->
        <div class="gallery-item">

          <img
            src="photo4.jpg"
            alt="व्यापार सभा लोगो फोटो"
            loading="lazy"
          >

          <p>व्यापार सभा लोगो</p>

        </div>

      </div>

    </div>

  </section>


  <!-- MEMBERSHIP -->
  <section class="membership" id="membership">

    <div class="container">

      <div class="section-title">

        <h2>व्यापार सभा से जुड़ें</h2>

        <p>
          ऑनलाइन सदस्यता आवेदन के लिए नीचे फॉर्म भरें।
        </p>

      </div>


      <div class="form-box">

        <form
          action="mailto:shivy.yadav1994@gmail.com"
          method="post"
          enctype="text/plain"
        >

          <div class="form-row">

            <div>

              <label>नाम</label>

              <input
                type="text"
                name="नाम"
                placeholder="अपना नाम लिखें"
                required
              >

            </div>


            <div>

              <label>मोबाइल नंबर</label>

              <input
                type="tel"
                name="मोबाइल"
                placeholder="मोबाइल नंबर"
                required
              >

            </div>

          </div>


          <label>व्यवसाय / दुकान का नाम</label>

          <input
            type="text"
            name="व्यवसाय"
            placeholder="व्यवसाय का नाम"
          >


          <label>पता</label>

          <textarea
            name="पता"
            placeholder="अपना पता लिखें"
          ></textarea>


          <button class="btn" type="submit">
            सदस्यता आवेदन भेजें
          </button>

        </form>

      </div>

    </div>

  </section>


  <!-- CONTACT -->
  <section class="contact" id="contact">

    <div class="container">

      <h2>संपर्क करें</h2>

      <p>
        व्यापार सभा नोएडा महानगर
      </p>

      <p>
        📍 नोएडा, उत्तर प्रदेश
      </p>

      <p>
        📧 shivy.yadav1994@gmail.com
      </p>

    </div>

  </section>


  <!-- FOOTER -->
  <footer>

    <p>
      © 2026 व्यापार सभा नोएडा महानगर | सर्वाधिकार सुरक्षित
    </p>

  </footer>

</body>
</html>
