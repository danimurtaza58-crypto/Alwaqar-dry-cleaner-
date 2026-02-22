# Alwaqar-dry-cleaner-<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Al Waqar Dry Cleaner</title>

<style>
* {margin:0;padding:0;box-sizing:border-box;font-family:sans-serif;}
body {background:#f5f7fa;color:#333;}

header {
  background:#0077b6;
  color:white;
  padding:15px 20px;
  display:flex;
  justify-content:space-between;
}

nav a {
  color:white;
  margin:0 10px;
  text-decoration:none;
}

.hero {
  height:90vh;
  background:linear-gradient(to right,#00b4d8,#90e0ef);
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
}

.btn {
  padding:12px 25px;
  margin:8px;
  border:none;
  border-radius:25px;
  background:#023e8a;
  color:white;
  cursor:pointer;
}

.section {padding:60px 20px;text-align:center;}

.services {
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
  gap:20px;
}

.box {
  background:white;
  padding:20px;
  border-radius:12px;
  box-shadow:0 5px 10px rgba(0,0,0,0.1);
}

form {
  max-width:400px;
  margin:auto;
}

input,textarea {
  width:100%;
  margin:10px 0;
  padding:12px;
  border-radius:8px;
  border:1px solid #ccc;
}

iframe {
  width:100%;
  height:300px;
  border:0;
  margin-top:20px;
}

footer {
  background:#023e8a;
  color:white;
  padding:20px;
  text-align:center;
}

.whatsapp {
  position:fixed;
  bottom:20px;
  right:20px;
  background:#25d366;
  padding:15px;
  border-radius:50%;
  color:white;
  text-decoration:none;
}

</style>

<script>
function sendToWhatsApp(event){
  event.preventDefault();

  let name = document.getElementById("name").value;
  let phone = document.getElementById("phone").value;
  let service = document.getElementById("service").value;

  let message = `Name: ${name}%0APhone: ${phone}%0AService: ${service}`;

  let whatsappNumber = "923477268985"; // your WhatsApp number

  let url = `https://wa.me/${whatsappNumber}?text=${message}`;
  window.open(url, "_blank");
}
</script>

</head>

<body>

<header>
  <h2>Al Waqar Dry Cleaner</h2>
  <nav>
    <a href="#">Home</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<div class="hero">
  <h1>Professional Dry Cleaning in Hazro</h1>
  <p>Fast, affordable & reliable service</p>
  
  <a href="tel:03477268985"><button class="btn">📞 Call Now</button></a>
  <a href="#contact"><button class="btn">Book Service</button></a>
</div>

<div class="section" id="services">
  <h2>Our Services</h2>
  <div class="services">
    <div class="box">🧥 Dry Cleaning</div>
    <div class="box">👕 Laundry Wash</div>
    <div class="box">🧼 Ironing</div>
    <div class="box">🛏️ Curtains & Blankets</div>
  </div>
</div>

<div class="section" id="contact">
  <h2>Book via WhatsApp</h2>

  <form onsubmit="sendToWhatsApp(event)">
    <input id="name" type="text" placeholder="Your Name" required>
    <input id="phone" type="tel" placeholder="Phone Number" required>
    <textarea id="service" placeholder="What do you want cleaned?" required></textarea>
    <button class="btn">Send Booking</button>
  </form>

  <p style="margin-top:20px;">📞 03477268985</p>
  <p>📍 G13-1 Street 108, Shop #11, Hazro</p>

  <!-- Google Map -->
  <iframe src="https://maps.google.com/maps?q=G13-1%20Street%20108%20Shop%20%2311%20Hazro&t=&z=17&ie=UTF8&iwloc=&output=embed"></iframe>

</div>

<footer>
  <p>© 2026 Al Waqar Dry Cleaner</p>
</footer>

<a class="whatsapp" href="https://wa.me/923477268985" target="_blank">💬</a>

</body>
</html>
