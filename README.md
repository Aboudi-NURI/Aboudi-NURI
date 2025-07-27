- 👋 Hi, I’m @Aboudi-NURI
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Aboudi-NURI/Aboudi-NURI is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
  background-color: #f5f7fa;
  color: #333;
}

header {
  background: #1f2937;
  padding: 1rem 2rem;
}

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #fff;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}

.nav-links a {
  color: #fff;
  text-decoration: none;
  transition: color 0.3s;
}

.nav-links a:hover {
  color: #00bcd4;
}

.hero {
  background: linear-gradient(135deg, #00bcd4, #2196f3);
  color: white;
  text-align: center;
  padding: 5rem 2rem;
}

.hero button {
  margin-top: 2rem;
  padding: 0.75rem 1.5rem;
  background: #fff;
  color: #2196f3;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-weight: bold;
}

.about, .contact {
  padding: 4rem 2rem;
  max-width: 800px;
  margin: auto;
}

.contact form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.contact input, .contact textarea {
  padding: 0.75rem;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.contact button {
  background: #2196f3;
  color: white;
  padding: 0.75rem;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

footer {
  background: #1f2937;
  color: white;
  text-align: center;
  padding: 1rem;
  margin-top: 2rem;
}

@media (max-width: 768px) {
  .nav-links {
    flex-direction: column;
    gap: 1rem;
  }
}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Awesome Site</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>

  <header>
    <nav class="navbar">
      <div class="logo">⭐ MySite</div>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="hero">
    <h1>Welcome to My Awesome Website</h1>
    <p>Built with HTML + CSS + JavaScript 🔨🤖🔧</p>
    <button onclick="scrollToSection('about')">Learn More</button>
  </section>

  <section id="about" class="about">
    <h2>About This Site</h2>
    <p>This site is fully responsive, smooth scrolling, and built from scratch.</p>
  </section>

  <section id="contact" class="contact">
    <h2>Contact Me</h2>
    <form id="contactForm">
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 MySite. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
function scrollToSection(id) {
  document.getElementById(id).scrollIntoView({
    behavior: 'smooth'
  });
}

document.getElementById('contactForm').addEventListener('submit', function (e) {
  e.preventDefault();
  alert('Thank you for your message! 😄');
  this.reset();
});
📁 styled-website
├── index.html
├── styles.css
└── script.js