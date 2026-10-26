
<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#f8c8d8">
<meta name="description" content="Mail BNK48 Fanpage — พื้นที่เก็บเรื่องราว ผลงาน และความทรงจำของเมล">
<title>Mail BNK48 | Sweet Scoop of Mail</title>

<style>
:root {
  --pink: #f8c8d8;
  --rose: #e99ab5;
  --dark-pink: #a64f70;
  --white: #ffffff;
  --milk: #fff5f8;
  --text: #57434b;
  --muted: #967d87;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html { scroll-behavior: smooth; }

body {
  font-family: "Tahoma", sans-serif;
  background: var(--milk);
  color: var(--text);
  line-height: 1.8;
}

a {
  color: inherit;
  text-decoration: none;
}

header {
  background: rgba(255,255,255,.96);
  padding: 15px 6%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 12px;
  flex-wrap: wrap;
  border-bottom: 1px solid #f5dce5;
  position: sticky;
  top: 0;
  z-index: 10;
}

.logo {
  font-weight: bold;
  color: var(--dark-pink);
  font-size: 19px;
}

nav {
  display: flex;
  gap: 15px;
  flex-wrap: wrap;
  font-size: 13px;
}

nav a:hover { color: var(--dark-pink); }

.hero {
  padding: 65px 20px;
  text-align: center;
  background:
    radial-gradient(circle at 15% 20%, #fff 0 5%, transparent 6%),
    radial-gradient(circle at 85% 75%, #fff 0 7%, transparent 8%),
    linear-gradient(135deg, #f8c8d8, #fff5f8 65%, #ffffff);
}

.hero .eyebrow {
  color: var(--dark-pink);
  letter-spacing: 3px;
  font-size: 12px;
  text-transform: uppercase;
}

.hero h1 {
  font-family: Georgia, serif;
  font-size: clamp(38px, 8vw, 65px);
  line-height: 1.25;
  color: var(--dark-pink);
  margin: 15px 0;
}

.hero p {
  max-width: 480px;
  margin: auto;
  font-size: 14px;
}

.hero .button {
  display: inline-block;
  margin-top: 25px;
  background: var(--dark-pink);
  color: white;
  padding: 10px 24px;
  border-radius: 30px;
  font-size: 14px;
}

section {
  padding: 55px 6%;
  max-width: 1100px;
  margin: auto;
}

.section-heading {
  text-align: center;
  margin-bottom: 28px;
}

.section-heading .en {
  font-size: 11px;
  color: var(--rose);
  letter-spacing: 3px;
}

.section-heading h2 {
  font-size: 27px;
  color: var(--dark-pink);
  margin-top: 4px;
}

.card {
  background: var(--white);
  padding: 24px;
  border: 1px solid #f3dce5;
  border-radius: 22px;
  box-shadow: 0 8px 25px rgba(166,79,112,.05);
}

.profile {
  display: grid;
  grid-template-columns: 1fr 1.2fr;
  gap: 25px;
  align-items: stretch;
}

.profile-cover {
  min-height: 300px;
  border-radius: 22px;
  background: linear-gradient(150deg, #f8c8d8, #fff);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 20px;
  color: var(--dark-pink);
}

.profile-cover .icon {
  font-size: 70px;
  margin-bottom: 10px;
}

.profile-cover p {
  font-size: 12px;
}

.profile h3 {
  font-size: 23px;
  color: var(--dark-pink);
  margin-bottom: 15px;
}

.info {
  display: grid;
  grid-template-columns: 115px 1fr;
  gap: 10px 12px;
  font-size: 14px;
}

.info dt { color: var(--muted); }
.info dd { overflow-wrap: anywhere; }

.note {
  margin-top: 18px;
  padding: 12px;
  background: var(--milk);
  border-radius: 12px;
  font-size: 12px;
  color: var(--muted);
}

.grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 16px;
}

.mini-card {
  background: white;
  padding: 22px;
  border-radius: 18px;
  border: 1px solid #f3dce5;
}

.mini-card .symbol {
  font-size: 25px;
}

.mini-card h3 {
  color: var(--dark-pink);
  font-size: 17px;
  margin: 7px 0;
}

.mini-card p {
  font-size: 13px;
  color: var(--muted);
  overflow-wrap: anywhere;
}

.work-list {
  display: grid;
  gap: 12px;
}

.work-item {
  display: flex;
  align-items: flex-start;
  gap: 14px;
  background: white;
  padding: 17px;
  border-radius: 15px;
  border: 1px solid #f3dce5;
}

.work-item .symbol { font-size: 23px; }
.work-item h3 { font-size: 15px; color: var(--dark-pink); }
.work-item p { font-size: 12px; color: var(--muted); }

.socials {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 15px;
}

.socials a {
  background: var(--milk);
  color: var(--dark-pink);
  border: 1px solid #f1d5e0;
  padding: 9px 15px;
  border-radius: 30px;
  font-size: 13px;
}

.socials a:hover {
  background: var(--pink);
}

footer {
  text-align: center;
  padding: 35px 20px;
  background: white;
  border-top: 1px solid #f3dce5;
  font-size: 12px;
  color: var(--muted);
}

footer strong { color: var(--dark-pink); }

@media (max-width: 650px) {
  header { justify-content: center; }
  nav { justify-content: center; gap: 12px; }
  .hero { padding: 55px 20px; }
  section { padding: 42px 18px; }
  .profile { grid-template-columns: 1fr; }
  .profile-cover { min-height: 200px; }
  .grid { grid-template-columns: 1fr; }
  .info { grid-template-columns: 105px 1fr; }
}
</style>
</head>

<body>

<header>
  <a class="logo" href="#home">♡ MAIL BNK48</a>
  <nav>
    <a href="#about">About</a>
    <a href="#interests">Interests</a>
    <a href="#works">Works</a>
    <a href="#follow">Follow</a>
  </nav>
</header>

<main>

<section class="hero" id="home">
  <p class="eyebrow">A Fanpage Dedicated to Mail</p>
  <h1>Sweet Scoop<br>of Mail ♡</h1>
  <p>
    Every scoop holds a memory.<br>
    พื้นที่เล็ก ๆ ที่รวบรวมเรื่องราว ผลงาน
    และความทรงจำดี ๆ ของเมล BNK48
  </p>
  <a class="button" href="#about">Discover Mail ♡</a>
</section>

<section id="about">
  <div class="section-heading">
    <p class="en">A LITTLE INTRODUCTION</p>
    <h2>About Mail</h2>
  </div>

  <div class="profile">
    <div class="profile-cover">
      <div class="icon">🍓</div>
      <h2>Mail BNK48</h2>
      <p>Strawberry sweetness in every moment.</p>
      <!-- เพิ่มภาพเมลที่ได้รับอนุญาตให้ใช้งานได้ตรงนี้ -->
    </div>

    <div class="card">
      <h3>Meet Mail ♡</h3>
      <dl class="info">
        <dt>ชื่อจริง</dt>
        <dd>รออัปเดตข้อมูลยืนยัน</dd>

        <dt>ชื่อในวง</dt>
        <dd>เมล (Mail)</dd>

        <dt>วันเกิด</dt>
        <dd>17 กรกฎาคม 2010</dd>

        <dt>อายุ</dt>
        <dd id="age">กำลังคำนวณ...</dd>

        <dt>ภูมิลำเนา</dt>
        <dd>รออัปเดตข้อมูลยืนยัน</dd>

        <dt>สิ่งที่ชอบ</dt>
        <dd>รออัปเดตข้อมูลยืนยัน</dd>

        <dt>งานอดิเรก</dt>
        <dd>รออัปเดตข้อมูลยืนยัน</dd>
      </dl>

      <p class="note">
        เว็บไซต์แฟนคลับจัดทำขึ้นเพื่อสนับสนุนเมล
        ข้อมูลที่ยังไม่ยืนยันจะไม่ระบุเป็นข้อเท็จจริง
      </p>
    </div>
  </div>
</section>

<section id="interests">
  <div class="section-heading">
    <p class="en">LITTLE THINGS ABOUT MAIL</p>
    <h2>Mail's Corner ♡</h2>
  </div>

  <div class="grid">
    <article class="mini-card">
      <div class="symbol">🍰</div>
      <h3>Things She Loves</h3>
      <p>รวมสิ่งที่เมลชอบ สีโปรด อาหารโปรด และสิ่งน่ารัก ๆ</p>
    </article>

    <article class="mini-card">
      <div class="symbol">🎀</div>
      <h3>Her Hobbies</h3>
      <p>งานอดิเรก ความสามารถ และเรื่องราวที่ทำให้เมลเป็นเมล</p>
    </article>

    <article class="mini-card">
      <div class="symbol">📸</div>
      <h3>Sweet Memories</h3>
      <p>ภาพและความทรงจำจากกิจกรรมต่าง ๆ ที่แฟนคลับประทับใจ</p>
    </article>

    <article class="mini-card">
      <div class="symbol">💌</div>
      <h3>Our Support</h3>
      <p>พื้นที่ส่งกำลังใจและร่วมสนับสนุนเมลไปด้วยกัน</p>
    </article>
  </div>
</section>

<section id="works">
  <div class="section-heading">
    <p class="en">HER JOURNEY</p>
    <h2>Works & Memories</h2>
  </div>

  <div class="work-list">
    <article class="work-item">
      <div class="symbol">🎤</div>
      <div>
        <h3>Music & Performances</h3>
        <p>รวบรวมเพลง การแสดง และผลงานของเมล</p>
      </div>
    </article>

    <article class="work-item">
      <div class="symbol">📅</div>
      <div>
        <h3>Events & Activities</h3>
        <p>ตารางกิจกรรม งานอีเวนต์ และประกาศต่าง ๆ</p>
      </div>
    </article>

    <article class="work-item">
      <div class="symbol">🌷</div>
      <div>
        <h3>Milestones</h3>
        <p>บันทึกเส้นทางและช่วงเวลาสำคัญของเมล</p>
      </div>
    </article>
  </div>

  <p class="note">
    หมายเหตุ: ส่วนผลงานเป็นหมวดสำหรับเติมข้อมูล
    ยังไม่ได้ระบุรายชื่อเพลงหรือผลงานเฉพาะที่ตรวจสอบแล้ว
  </p>
</section>

<section id="follow">
  <div class="section-heading">
    <p class="en">STAY CONNECTED</p>
    <h2>Follow Mail ♡</h2>
  </div>

  <div class="card">
    <p>
      ติดตามข่าวสารและความเคลื่อนไหวของเมล
      ผ่านช่องทางอย่างเป็นทางการ
    </p>

    <div class="socials">
      <a href="https://www.bnk48.com/?page=members"
         target="_blank" rel="noopener noreferrer">
        BNK48 Official Website ↗
      </a>
      <!-- เพิ่มลิงก์โซเชียลทางการของเมลเมื่อยืนยันแล้ว -->
    </div>
  </div>

  <div class="card" style="margin-top:18px">
    <h3 style="color:var(--dark-pink)">Our Community ♡</h3>
    <p style="font-size:14px;margin-top:8px">
      พื้นที่สำหรับผู้ที่รักและสนับสนุนเมล
      ติดตามข่าวสาร กิจกรรม และโปรเจกต์จากบ้านแฟนคลับ
    </p>
    <div class="socials">
      <!-- ใส่ลิงก์บ้านแฟนคลับ -->
      <a href="#follow">Fanbase channels — Coming soon</a>
    </div>
  </div>
</section>

</main>

<footer>
  <p><strong>Mail BNK48 Fanpage ♡</strong></p>
  <p>Sweet Scoop of Mail · Made with love by fans</p>
  <p>Unofficial fan-made website. Not affiliated with BNK48.</p>
  <p>© <span id="year"></span> Mail Fanpage</p>
</footer>

<script>
function calculateAge() {
  // ใช้ปี ค.ศ. เดือน และวันเกิดจริง
  // เดือนใน JavaScript เริ่มนับจาก 0
  const birthDate = new Date(2010, 6, 17);
  const now = new Date();

  let age = now.getFullYear() - birthDate.getFullYear();

  const birthdayHasPassed =
    now.getMonth() > birthDate.getMonth() ||
    (now.getMonth() === birthDate.getMonth() &&
     now.getDate() >= birthDate.getDate());

  if (!birthdayHasPassed) age--;

  const ageElement = document.getElementById("age");

  if (now < birthDate) {
    ageElement.textContent = "รอยืนยันวันเกิด";
  } else {
    ageElement.textContent = age + " ปี";
  }
}

calculateAge();

document.getElementById("year").textContent =
  new Date().getFullYear();
</script>

</body>
</html>