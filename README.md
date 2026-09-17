<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Narumon Sopin | Portfolio</title>

<style>
:root {
  --navy: #17263a;
  --navy2: #22364f;
  --slate: #617084;
  --light: #f4f6f8;
  --white: #ffffff;
  --line: #dce2e8;
  --accent: #9bb2c8;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: "Noto Sans Thai", Tahoma, Arial, sans-serif;
  color: var(--navy);
  background: #f7f8fa;
  line-height: 1.75;
}

a {
  text-decoration: none;
  color: inherit;
}

/* NAVIGATION */
nav {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 10;

  background: rgba(255,255,255,0.92);
  backdrop-filter: blur(14px);

  border-bottom: 1px solid var(--line);
}

.nav-inner {
  max-width: 1120px;
  margin: auto;
  padding: 15px 24px;

  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-weight: 800;
  letter-spacing: 1px;
}

.logo span {
  color: var(--slate);
}

.nav-links {
  display: flex;
  gap: 25px;
  font-size: 14px;
  color: #536174;
}

.nav-links a:hover {
  color: var(--navy);
}


/* SECTION */
section {
  max-width: 1120px;
  margin: auto;
  padding: 95px 24px;
}


/* HERO */
.hero {
  min-height: 100vh;

  display: grid;
  grid-template-columns: 1.1fr 0.9fr;

  align-items: center;
  gap: 60px;

  padding-top: 120px;
}

.eyebrow {
  display: inline-block;

  border: 1px solid #cbd5df;
  border-radius: 999px;

  padding: 6px 14px;

  font-size: 13px;
  color: var(--slate);

  margin-bottom: 18px;

  background: #fff;
}

h1 {
  font-size: clamp(42px, 7vw, 76px);

  line-height: 1.05;
  letter-spacing: -2px;

  margin-bottom: 18px;
}

.hero h1 span {
  color: #6e8297;
}

.subtitle {
  font-size: 20px;
  font-weight: 700;

  margin-bottom: 15px;
}

.hero p {
  max-width: 650px;

  color: #5c6978;
  font-size: 17px;
}


/* BUTTON */
.buttons {
  display: flex;
  gap: 12px;

  margin-top: 28px;
  flex-wrap: wrap;
}

.btn {
  padding: 11px 20px;

  border-radius: 10px;

  font-weight: 700;
  font-size: 14px;

  border: 1px solid var(--navy);
}

.btn.primary {
  background: var(--navy);
  color: #fff;
}

.btn.secondary {
  background: #fff;
  color: var(--navy);
  border-color: var(--line);
}


/* PROFILE */
.profile-wrap {
  display: flex;
  justify-content: center;
}

.profile-card {
  width: min(360px, 85vw);

  padding: 12px;

  background: #fff;

  border: 1px solid var(--line);
  border-radius: 28px;

  box-shadow:
    0 22px 55px rgba(23,38,58,0.12);

  transform: rotate(2deg);
}

.profile-card img {
  width: 100%;

  aspect-ratio: 1 / 1;

  object-fit: cover;
  object-position: center 32%;

  border-radius: 20px;

  display: block;
}

.caption {
  padding: 14px 8px 4px;

  text-align: center;

  font-size: 13px;

  color: var(--slate);

  transform: rotate(-2deg);
}


/* ABOUT */
.about {
  background: #fff;

  border-top: 1px solid var(--line);
  border-bottom: 1px solid var(--line);

  max-width: none;
}

.about-inner {
  max-width: 1120px;
  margin: auto;

  padding: 95px 24px;
}

.about-grid {
  display: grid;

  grid-template-columns: 0.75fr 1.25fr;

  gap: 60px;
}

.about-text {
  color: #5b6877;
}

.about-text p + p {
  margin-top: 16px;
}


/* SECTION HEAD */
.section-head {
  margin-bottom: 35px;
}

.kicker {
  text-transform: uppercase;

  letter-spacing: 2px;

  font-size: 12px;

  color: var(--slate);

  font-weight: 800;
}

.section-head h2 {
  font-size: 36px;

  line-height: 1.2;

  margin-top: 6px;
}


/* SKILLS */
.skills {
  display: grid;

  grid-template-columns: repeat(3, 1fr);

  gap: 15px;

  margin-top: 28px;
}

.skill {
  padding: 22px;

  background: #f7f8fa;

  border: 1px solid var(--line);

  border-radius: 16px;
}

.skill strong {
  display: block;

  margin-bottom: 5px;
}

.skill small {
  color: var(--slate);
}


/* CONTACT */
.contact {
  background: var(--navy);

  color: #fff;

  max-width: none;
}

.contact-inner {
  max-width: 1120px;
  margin: auto;

  padding: 85px 24px;

  display: flex;

  justify-content: space-between;

  gap: 40px;

  align-items: center;
}

.contact p {
  color: #cbd4de;

  margin-top: 8px;
}

.socials {
  display: flex;

  gap: 10px;

  flex-wrap: wrap;
}

.social {
  border: 1px solid #52657a;

  padding: 10px 15px;

  border-radius: 10px;

  font-size: 14px;
}

.social:hover {
  background: #22364f;
}


/* FOOTER */
footer {
  text-align: center;

  padding: 20px;

  color: #8491a0;

  background: #101c2b;

  font-size: 12px;
}


/* MOBILE */
@media (max-width: 780px) {

  .nav-links {
    display: none;
  }

  .hero {
    grid-template-columns: 1fr;

    text-align: center;

    gap: 35px;
  }

  .hero p {
    margin: auto;
  }

  .buttons {
    justify-content: center;
  }

  .about-grid {
    grid-template-columns: 1fr;

    gap: 25px;
  }

  .skills {
    grid-template-columns: 1fr;
  }

  .contact-inner {
    flex-direction: column;

    align-items: flex-start;
  }

  .profile-card {
    transform: none;
  }
}
</style>
</head>


<body>


<!-- ================= NAVBAR ================= -->

<nav>

  <div class="nav-inner">

    <div class="logo">
      NRM<span>.</span>
    </div>

    <div class="nav-links">

      <a href="#about">
        About
      </a>

      <a href="#skills">
        Skills
      </a>

      <a href="#contact">
        Contact
      </a>

    </div>

  </div>

</nav>



<!-- ================= HERO ================= -->

<main>

<section class="hero">

  <div>

    <div class="eyebrow">
      PORTFOLIO · OCCUPATIONAL HEALTH & SAFETY
    </div>


    <h1>
      Narumon
      <br>
      <span>Sopin</span>
    </h1>


    <div class="subtitle">
      นางสาวนฤมล โสพิน · “ส้ม”
    </div>


    <p>
      นักศึกษาคณะสาธารณสุขศาสตร์
      สาขาอาชีวอนามัยและความปลอดภัย
      ผู้มุ่งมั่นเรียนรู้และพัฒนาตนเองอยู่เสมอ
      สนใจการแก้ปัญหาอย่างเป็นระบบ
      และการนำเทคโนโลยีมาประยุกต์ใช้กับงานจริง
    </p>


    <div class="buttons">

      <a
        class="btn primary"
        href="#skills"
      >
        ดูทักษะ
      </a>


      <a
        class="btn secondary"
        href="#contact"
      >
        ติดต่อฉัน
      </a>

    </div>

  </div>



  <!-- PROFILE IMAGE -->

  <div class="profile-wrap">

    <div class="profile-card">

      <img
        src="IMG_4677.jpeg"
        alt="Narumon profile photo"
      >

      <div class="caption">
        Narumon Sopin · Student Portfolio
      </div>

    </div>

  </div>

</section>



<!-- ================= ABOUT ================= -->

<div class="about" id="about">

  <div class="about-inner">

    <section style="padding:0">

      <div class="about-grid">


        <div class="section-head">

          <div class="kicker">
            01 · About Me
          </div>

          <h2>
            ความมุ่งมั่น
            <br>
            และความสนใจ
          </h2>

        </div>



        <div class="about-text">

          <p>
            ฉันชื่อ นฤมล โสพิน
            ชื่อเล่น “ส้ม”
            ปัจจุบันเป็นนักศึกษาชั้นปีที่ 1
            สาขาอาชีวอนามัยและความปลอดภัย
            คณะสาธารณสุขศาสตร์
            มีความสนใจในการแก้ปัญหาเชิงตรรกะ
            การเรียนรู้เทคโนโลยี
            และการพัฒนาทักษะที่สามารถนำไปประยุกต์ใช้กับการทำงานจริง
          </p>


          <p>
            ฉันมีความกระตือรือร้นในการเรียนรู้
            เปิดรับคำแนะนำ
            และพร้อมนำข้อเสนอแนะมาพัฒนาตนเองให้ดีขึ้น
            สามารถทำงานเป็นทีมได้ดีและทำงานอย่างรวดเร็ว
            ปัจจุบันกำลังมองหาโอกาสฝึกงานหรือสหกิจศึกษา
            เพื่อเรียนรู้จากโจทย์จริง
            และนำความรู้จากห้องเรียนไปประยุกต์ใช้ในภาคอุตสาหกรรม
          </p>

        </div>

      </div>

    </section>

  </div>

</div>



<!-- ================= SKILLS ================= -->

<section id="skills">

  <div class="section-head">

    <div class="kicker">
      02 · Skills
    </div>

    <h2>
      ทักษะและความสามารถ
    </h2>

  </div>



  <div class="skills">


    <div class="skill">

      <strong>
        Teamwork
      </strong>

      <small>
        ทำงานร่วมกับผู้อื่น
        และแบ่งหน้าที่อย่างเป็นระบบ
      </small>

    </div>



    <div class="skill">

      <strong>
        Fast Learner
      </strong>

      <small>
        เรียนรู้สิ่งใหม่
        และปรับตัวกับงานได้รวดเร็ว
      </small>

    </div>



    <div class="skill">

      <strong>
        Problem Solving
      </strong>

      <small>
        สนใจการแก้ปัญหาเชิงตรรกะ
        และคิดอย่างเป็นขั้นตอน
      </small>

    </div>


  </div>

</section>



<!-- ================= CONTACT ================= -->

<div class="contact" id="contact">

  <div class="contact-inner">


    <div>

      <div
        class="kicker"
        style="color:#9fb0c2"
      >
        03 · Contact
      </div>


      <h2>
        Let's connect.
      </h2>


      <p>
        เปิดรับโอกาสในการเรียนรู้
        ฝึกงาน
        และทำงานร่วมกับผู้อื่น
      </p>

    </div>



    <div class="socials">


      <a
        class="social"
        href="https://www.facebook.com/"
        target="_blank"
      >
        Facebook · นฤมลฯ
      </a>


      <a
        class="social"
        href="https://www.instagram.com/naruemon.inc/"
        target="_blank"
      >
        Instagram · @naruemon.inc
      </a>


    </div>

  </div>

</div>


</main>



<!-- ================= FOOTER ================= -->

<footer>

  © 2026 Narumon Sopin · Portfolio

</footer>


</body>
</html>
