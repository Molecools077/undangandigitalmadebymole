
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Wedding of Alex & Amanda</title>

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600&family=Montserrat:wght@300;400;500&display=swap" rel="stylesheet">

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --cream: #f8f5ef;
  --gold: #a58b60;
  --dark: #39362f;
}

body {
  background: var(--cream);
  color: var(--dark);
  font-family: 'Montserrat', sans-serif;
  font-weight: 300;
}

html {
  scroll-behavior: smooth;
}

h1, h2, h3 {
  font-family: 'Cormorant Garamond', serif;
  font-weight: 400;
}

section {
  padding: 90px 20px;
  text-align: center;
}

.eyebrow {
  font-size: 10px;
  letter-spacing: 4px;
  color: var(--gold);
  text-transform: uppercase;
}

.heading {
  font-size: 55px;
  margin: 20px 0;
}

.description {
  max-width: 500px;
  margin: auto;
  font-size: 12px;
  line-height: 2;
  color: #817b70;
}

button {
  cursor: pointer;
  font-family: inherit;
}

/* COVER */

.cover {
  height: 100vh;
  min-height: 650px;
  background:
    linear-gradient(#0005,#0007),
    url('assets/cover.jpg') center/cover;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  padding: 25px;
}

.cover-content {
  border: 1px solid #ffffff90;
  width: 100%;
  max-width: 600px;
  padding: 70px 20px;
}

.cover h1 {
  font-size: clamp(65px, 12vw, 100px);
  line-height: .85;
  margin: 30px 0;
}

.cover .eyebrow {
  color: #ead8b7;
}

.cover-date {
  letter-spacing: 4px;
  font-size: 11px;
}

.btn {
  padding: 15px 30px;
  background: var(--gold);
  color: white;
  border: 1px solid var(--gold);
  font-size: 10px;
  letter-spacing: 2px;
  margin-top: 30px;
}

.btn:hover {
  opacity: .8;
}

/* INTRO */

.intro {
  background: #fffdfa;
}

.monogram {
  font-family: 'Cormorant Garamond';
  font-size: 55px;
  color: var(--gold);
}

.names {
  font-size: 55px;
  line-height: 1;
  margin: 35px 0;
}

.amp {
  color: var(--gold);
  font-style: italic;
}

.couple {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 25px;
  max-width: 750px;
  margin: 50px auto 0;
}

.couple img {
  width: 100%;
  height: 380px;
  object-fit: cover;
}

.couple h3 {
  font-size: 32px;
  margin-top: 15px;
}

.couple p {
  font-size: 11px;
  line-height: 2;
  color: #817b70;
  margin-top: 8px;
}

/* COUNTDOWN */

.countdown {
  background: #eae3d8;
}

.timer {
  display: flex;
  justify-content: center;
  gap: 35px;
  margin-top: 40px;
}

.timer strong {
  font-family: 'Cormorant Garamond';
  font-size: 55px;
  display: block;
}

.timer span {
  font-size: 9px;
  letter-spacing: 2px;
}

/* EVENTS */

.events {
  background: var(--cream);
}

.event-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
  max-width: 800px;
  margin: 40px auto;
}

.event-card {
  background: white;
  padding: 40px 20px;
  border: 1px solid #e4dbce;
}

.event-card h3 {
  font-size: 35px;
  margin: 15px;
}

.event-card p {
  font-size: 12px;
  line-height: 2;
  color: #817b70;
}

/* GALLERY */

.gallery {
  background: white;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(3,1fr);
  gap: 12px;
  max-width: 900px;
  margin: 40px auto;
}

.gallery-grid img {
  width: 100%;
  height: 280px;
  object-fit: cover;
  cursor: pointer;
}

/* RSVP */

.rsvp {
  background: white;
}

form {
  max-width: 450px;
  margin: 40px auto;
  text-align: left;
}

input, select, textarea {
  width: 100%;
  padding: 15px;
  border: 1px solid #ddd3c5;
  background: transparent;
  margin: 10px 0 20px;
  font-family: inherit;
}

label {
  font-size: 10px;
  letter-spacing: 2px;
  text-transform: uppercase;
}

form button {
  width: 100%;
}

/* GIFT */

.gift {
  background: #eae3d8;
}

.gift-card {
  max-width: 400px;
  background: white;
  padding: 40px;
  margin: 40px auto;
  border: 1px solid #ded3c3;
}

.account {
  font-size: 22px;
  letter-spacing: 2px;
  margin: 20px 0;
}

/* FOOTER */

footer {
  padding: 35px;
  text-align: center;
  font-size: 10px;
  letter-spacing: 2px;
  background: white;
}

/* MUSIC */

.music {
  position: fixed;
  right: 20px;
  bottom: 20px;
  width: 45px;
  height: 45px;
  border-radius: 50%;
  border: 1px solid var(--gold);
  background: white;
  color: var(--gold);
  z-index: 10;
}

/* RESPONSIVE */

@media(max-width:600px) {
  section {
    padding: 70px 18px;
  }

  .heading {
    font-size: 43px;
  }

  .names {
    font-size: 42px;
  }

  .couple img {
    height: 230px;
  }

  .couple {
    gap: 12px;
  }

  .event-grid {
    grid-template-columns: 1fr;
  }

  .gallery-grid {
    grid-template-columns: 1fr 1fr;
  }

  .gallery-grid img {
    height: 190px;
  }

  .timer {
    gap: 17px;
  }

  .timer strong {
    font-size: 38px;
  }
}
</style>
</head>

<body>

<!-- COVER -->
<section class="cover">
  <div class="cover-content">
    <div class="eyebrow">The Wedding Of</div>

    <h1>Alex<br>&<br>Amanda</h1>

    <div class="cover-date">
      SUNDAY, 20 JUNE 2027
    </div>

    <button class="btn" onclick="openInvitation()">
      OPEN INVITATION
    </button>
  </div>
</section>

<main id="invitation" hidden>

<!-- INTRO -->
<section class="intro">
  <div class="monogram">A & A</div>

  <div class="eyebrow">Together With Our Families</div>

  <p class="description" style="margin-top:20px">
    With joyful hearts, we invite you to celebrate
    the beginning of our forever.
  </p>

  <div class="names">
    Alex <span class="amp">&</span> Amanda
  </div>

  <p class="description">
    "And We created you in pairs."
    <br>— QS. An-Naba: 8
  </p>

  <div class="couple">

    <div>
      <img src="assets/groom.jpg" alt="Groom">
      <h3>Alex Anderson</h3>
      <p>
        Son of Mr. John Anderson<br>
        & Mrs. Jane Anderson
      </p>
    </div>

    <div>
      <img src="assets/bride.jpg" alt="Bride">
      <h3>Amanda Smith</h3>
      <p>
        Daughter of Mr. Robert Smith<br>
        & Mrs. Anna Smith
      </p>
    </div>

  </div>
</section>

<!-- COUNTDOWN -->
<section class="countdown">

  <div class="eyebrow">Save The Date</div>

  <h2 class="heading">Counting Down</h2>

  <p class="description">
    We can't wait to celebrate this special moment with you.
  </p>

  <div class="timer">

    <div>
      <strong id="days">00</strong>
      <span>DAYS</span>
    </div>

    <div>
      <strong id="hours">00</strong>
      <span>HOURS</span>
    </div>

    <div>
      <strong id="minutes">00</strong>
      <span>MINUTES</span>
    </div>

    <div>
      <strong id="seconds">00</strong>
      <span>SECONDS</span>
    </div>

  </div>
</section>

<!-- EVENTS -->
<section class="events">

  <div class="eyebrow">The Celebration</div>

  <h2 class="heading">Wedding Details</h2>

  <div class="event-grid">

    <div class="event-card">
      <div class="eyebrow">01 — Ceremony</div>
      <h3>Akad Nikah</h3>
      <p>
        Sunday, 20 June 2027<br>
        09.00 AM – 11.00 AM<br><br>
        The Grand Ballroom<br>
        Jakarta, Indonesia
      </p>
    </div>

    <div class="event-card">
      <div class="eyebrow">02 — Reception</div>
      <h3>Reception</h3>
      <p>
        Sunday, 20 June 2027<br>
        12.00 PM – 03.00 PM<br><br>
        The Grand Ballroom<br>
        Jakarta, Indonesia
      </p>
    </div>

  </div>

  <a href="https://maps.google.com"
     target="_blank"
     class="btn"
     style="display:inline-block;text-decoration:none">
    VIEW GOOGLE MAPS
  </a>

</section>

<!-- GALLERY -->
<section class="gallery">

  <div class="eyebrow">Our Moments</div>

  <h2 class="heading">Photo Gallery</h2>

  <p class="description">
    A little collection of our beautiful memories.
  </p>

  <div class="gallery-grid">
    <img src="assets/gallery-1.jpg" alt="Gallery 1">
    <img src="assets/gallery-2.jpg" alt="Gallery 2">
    <img src="assets/gallery-3.jpg" alt="Gallery 3">
    <img src="assets/gallery-4.jpg" alt="Gallery 4">
    <img src="assets/gallery-5.jpg" alt="Gallery 5">
    <img src="assets/gallery-6.jpg" alt="Gallery 6">
  </div>

</section>

<!-- RSVP -->
<section class="rsvp">

  <div class="eyebrow">Kindly Respond</div>

  <h2 class="heading">RSVP</h2>

  <p class="description">
    Your presence would mean the world to us.
  </p>

  <form id="rsvpForm">

    <label>Full Name</label>
    <input id="guestName" required placeholder="Your name">

    <label>Confirmation</label>
    <select id="attendance" required>
      <option value="">Select response</option>
      <option value="Hadir">Joyfully accepts</option>
      <option value="Tidak hadir">Regretfully declines</option>
    </select>

    <label>Number of Guests</label>
    <select id="guestCount">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
    </select>

    <label>Your Wishes</label>
    <textarea id="message" placeholder="Write your wishes..."></textarea>

    <button class="btn" type="submit">
      SEND RSVP VIA WHATSAPP
    </button>

  </form>

</section>

<!-- GIFT -->
<section class="gift">

  <div class="eyebrow">Wedding Gift</div>

  <h2 class="heading">Send Your Love</h2>

  <p class="description">
    Your prayers and presence are the greatest gifts.
  </p>

  <div class="gift-card">

    <div class="eyebrow">BANK NAME</div>

    <div class="account" id="accountNumber">
      1234567890
    </div>

    <p>AN. ALEX ANDERSON</p>

    <button class="btn" onclick="copyAccount()">
      COPY ACCOUNT NUMBER
    </button>

  </div>

</section>

<!-- CLOSING -->
<section>
  <div class="eyebrow">With Love</div>

  <h2 class="heading">
    See You On Our Special Day
  </h2>

  <p class="description">
    Thank you for being part of our story.
    We look forward to celebrating with you.
  </p>

  <div class="names">
    Alex <span class="amp">&</span> Amanda
  </div>
</section>

</main>

<footer>
  MADE WITH LOVE · ALEX & AMANDA · 2027
</footer>

<!-- MUSIC -->
<audio id="bgMusic" src="assets/music.mp3" loop></audio>

<button class="music" onclick="toggleMusic()" id="musicBtn">
  ♫
</button>

<script>

/* ==========================
   WEDDING CONFIGURATION
========================== */

const CONFIG = {

  weddingDate: "2027-06-20T09:00:00+07:00",

  whatsapp: "6281234567890",

  accountNumber: "1234567890"

};

/* OPEN INVITATION */

function openInvitation() {

  document.getElementById("invitation").hidden = false;

  document.getElementById("invitation")
    .scrollIntoView({behavior:"smooth"});

  document.getElementById("bgMusic").play()
    .catch(()=>{});

}

/* COUNTDOWN */

const targetDate = new Date(CONFIG.weddingDate).getTime();

function updateCountdown() {

  const now = Date.now();

  let distance = Math.max(0,targetDate-now);

  document.getElementById("days").innerText =
    Math.floor(distance/(1000*60*60*24));

  document.getElementById("hours").innerText =
    Math.floor((distance%(1000*60*60*24))/(1000*60*60));

  document.getElementById("minutes").innerText =
    Math.floor((distance%(1000*60*60))/(1000*60));

  document.getElementById("seconds").innerText =
    Math.floor((distance%(1000*60))/1000);

}

updateCountdown();
setInterval(updateCountdown,1000);

/* MUSIC */

function toggleMusic() {

  const music = document.getElementById("bgMusic");
  const btn = document.getElementById("musicBtn");

  if(music.paused) {

    music.play();
    btn.innerText = "♫";

  } else {

    music.pause();
    btn.innerText = "♪";

  }

}

/* RSVP WHATSAPP */

document.getElementById("rsvpForm")
.addEventListener("submit",function(e){

  e.preventDefault();

  const name =
    document.getElementById("guestName").value;

  const attendance =
    document.getElementById("attendance").value;

  const count =
    document.getElementById("guestCount").value;

  const message =
    document.getElementById("message").value;

  const text =
    `Wedding RSVP\n\n`+
    `Name: ${name}\n`+
    `Confirmation: ${attendance}\n`+
    `Guests: ${count}\n`+
    `Wishes: ${message}`;

  const url =
    `https://wa.me/${CONFIG.whatsapp}?text=${encodeURIComponent(text)}`;

  window.open(url,"_blank");

});

/* COPY ACCOUNT */

function copyAccount() {

  navigator.clipboard.writeText(CONFIG.accountNumber)
    .then(()=>alert("Account number copied!"))
    .catch(()=>alert("Unable to copy. Please copy manually."));

}

</script>

</body>
</html>
