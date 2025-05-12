<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Abhishek Coaching Centre</title>
  <link rel="stylesheet" href="style.css" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(to right, #e0f7fa, #e0f2f1);
    }header {
  background-color: #00796b;
  color: white;
  padding: 20px;
  text-align: center;
}

nav {
  display: flex;
  justify-content: center;
  gap: 20px;
  background: #004d40;
  padding: 10px;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: 600;
}

nav a:hover {
  text-decoration: underline;
}

section {
  padding: 60px 20px;
  max-width: 1000px;
  margin: auto;
}

.section-card {
  background: #ffffff;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
  padding: 40px;
  margin-bottom: 40px;
}

.section-card h2 {
  text-align: center;
  color: #00796b;
  font-size: 2.2rem;
  margin-bottom: 40px;
}

.pricing-vertical {
  display: flex;
  flex-direction: column;
  gap: 25px;
}

.pricing-card {
  position: relative;
  background: #fafafa;
  padding: 30px;
  border-radius: 12px;
  border: 1px solid #ccc;
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.05);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.pricing-card.popular {
  background-color: #e0f7fa;
  border: 2px solid #00796b;
}

.pricing-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 12px 20px rgba(0, 0, 0, 0.1);
}

.pricing-card h3 {
  color: #00796b;
  font-size: 1.7rem;
  margin-bottom: 10px;
}

.pricing-card .price {
  font-size: 2rem;
  color: #00796b;
  font-weight: bold;
  margin: 15px 0;
}

.pricing-card ul {
  list-style: none;
  padding: 0;
  margin-bottom: 20px;
}

.pricing-card ul li {
  margin: 10px 0;
  position: relative;
  padding-left: 20px;
}

.pricing-card ul li::before {
  content: "✓";
  position: absolute;
  left: 0;
  color: #00796b;
  font-weight: bold;
}

.enroll-btn {
  background-color: #00796b;
  color: white;
  border: none;
  padding: 12px 24px;
  border-radius: 8px;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.enroll-btn:hover {
  background-color: #004d40;
}

.popular-label {
  position: absolute;
  top: -10px;
  right: -10px;
  background: #ff9800;
  color: white;
  font-weight: bold;
  padding: 6px 12px;
  border-radius: 50px;
  font-size: 0.85rem;
}

form label, form input {
  display: block;
  width: 100%;
  margin-bottom: 15px;
}

form input {
  padding: 10px;
  border-radius: 6px;
  border: 1px solid #ccc;
}

.payment-button {
  background-color: #43a047;
  color: white;
  padding: 10px 20px;
  font-size: 1rem;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  margin-top: 20px;
}

.payment-button:hover {
  background-color: #2e7d32;
}

footer {
  background: #00796b;
  color: white;
  text-align: center;
  padding: 20px;
  margin-top: 40px;
}

  </style>
  <script src="https://checkout.razorpay.com/v1/checkout.js"></script>
</head>
<body>
  <header>
    <h1>Abhishek Coaching Centre</h1>
    <p>All Subjects Coaching for Classes 1–10</p>
  </header>  <nav>
    <a href="#about">About</a>
    <a href="#fees">Fees</a>
    <a href="#admission">Admission</a>
    <a href="#payment">Payment</a>
    <a href="#contact">Contact</a>
  </nav>  <section id="about" class="section-card">
    <h2>About Us</h2>
    <p>Abhishek Coaching Centre provides comprehensive tutoring for students of classes 1–10. With personalized teaching methods and experienced teachers, we help students succeed academically and build confidence.</p>
  </section>  <section id="fees" class="section-card">
    <h2>Tuition Fee Structure</h2>
    <div class="pricing-vertical">
      <div class="pricing-card">
        <h3>Basic</h3>
        <p class="price">₹2000/month</p>
        <p>For Classes 1–4</p>
        <ul>
          <li>Weekly 2 hours of classes</li>
          <li>Subject-specific focus</li>
          <li>Online support available</li>
        </ul>
        <button class="enroll-btn">Enroll Now</button>
      </div><div class="pricing-card popular">
    <h3>Standard</h3>
    <p class="price">₹3000/month</p>
    <p>For Classes 5–7</p>
    <ul>
      <li>Weekly 3 hours of classes</li>
      <li>Personalized doubt clearing</li>
      <li>Study material included</li>
    </ul>
    <button class="enroll-btn">Enroll Now</button>
    <span class="popular-label">Most Popular</span>
  </div>

  <div class="pricing-card">
    <h3>Premium</h3>
    <p class="price">₹4000/month</p>
    <p>For Classes 8–10</p>
    <ul>
      <li>Weekly 4 hours of classes</li>
      <li>Mock tests and assessments</li>
      <li>Personal tutoring</li>
    </ul>
    <button class="enroll-btn">Enroll Now</button>
  </div>
</div>

  </section>  <section id="admission" class="section-card">
    <h2>Admission Form</h2>
    <form>
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required>
      <label for="class">Class:</label>
      <input type="text" id="class" name="class" required>
      <label for="contact">Contact Number:</label>
      <input type="text" id="contact" name="contact" required>
      <button class="enroll-btn" type="submit">Submit</button>
    </form>
  </section>  <section id="payment" class="section-card">
    <h2>Online Payment</h2>
    <p>You can pay your tuition fees online using the button below. Secure payments powered by Razorpay/Paytm/Google Pay.</p>
    <button class="payment-button" onclick="window.location.href='https://www.examplepaymentgateway.com'">Pay Now</button>
  </section>  <section id="contact" class="section-card">
    <h2>Contact Us</h2>
    <p>Phone: 6291758913</p>
    <p>WhatsApp: pora</p>
    <p>Location: [Embed Google Map Here]</p>
  </section>  <footer>
    <p>&copy; 2025 Abhishek Coaching Centre. All rights reserved.</p>
  </footer>
  <section class="section-card">
  <h2>What Our Students Say</h2>
  <div class="testimonial">
    <p>"The classes are amazing! I improved a lot in math and science."</p>
    <strong>— Riya Das, Class 10</strong>
  </div>
  <div class="testimonial">
    <p>"Best coaching center in the area. Abhishek Sir explains everything so well!"</p>
    <strong>— Arjun Roy, Class 8</strong>
  </div>
</section>
<section class="section-card">
  <h2>Gallery</h2>
  <div style="display: flex; gap: 10px; flex-wrap: wrap;">
    <img src="photo1.jpg" alt="Classroom" width="150">
    <img src="photo2.jpg" alt="Teacher Abhishek Sir" width="150">
    <img src="photo3.jpg" alt="Student Activity" width="150">
  </div>
</section>
<section class="section-card">
  <h2>FAQs</h2>
  <p><strong>Q:</strong> What classes do you teach?<br><strong>A:</strong> Classes 6 to 10 - All subjects.</p>
  <p><strong>Q:</strong> What are the tuition timings?<br><strong>A:</strong> Morning and Evening Batches Available.</p>
</section>
<section class="section-card">
  <h2>Contact Us</h2>
  <form action="mailto:youremail@example.com" method="post" enctype="text/plain">
    <input type="text" name="name" placeholder="Your Name" required><br><br>
    <input type="email" name="email" placeholder="Your Email" required><br><br>
    <textarea name="message" placeholder="Your Message" rows="4" required></textarea><br><br>
    <button class="payment-button" type="submit">Send Message</button>
  </form>
</section>
<section class="section-card">
  <h2>Latest Announcements</h2>
  <marquee behavior="scroll" direction="left">New batch for Class 9 starts from 15th May. Limited seats available!</marquee>
</section>
<section class="section-card">
  <h2>Next Batch Starts In:</h2>
  <p id="countdown" style="font-size: 1.5rem; color: red;"></p>
</section>

<script>
  const targetDate = new Date("2025-06-01T00:00:00").getTime();
  const countdown = setInterval(() => {
    const now = new Date().getTime();
    const diff = targetDate - now;
    const days = Math.floor(diff / (1000 * 60 * 60 * 24));
    const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    const mins = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
    const secs = Math.floor((diff % (1000 * 60)) / 1000);
    document.getElementById("countdown").innerHTML = `${days}d ${hours}h ${mins}m ${secs}s`;
    if (diff < 0) {
      clearInterval(countdown);
      document.getElementById("countdown").innerHTML = "Batch Started!";
    }
  }, 1000);
</script>
<section class="section-card">
  <h2>Student Success Stories</h2>
  <div>
    <p><strong>Suman Roy:</strong> Scored 95% in Madhyamik after 1 year with us.</p>
    <p><strong>Puja Das:</strong> From 60% to 88% in just 6 months!</p>
  </div>
</section>
<section class="section-card">
  <h2>Find Us on Map</h2>
  <iframe 
    src="https://www.google.com/maps/embed?pb=YOUR_MAP_EMBED_LINK" 
    width="100%" height="300" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
</section>
</body>
</html>
