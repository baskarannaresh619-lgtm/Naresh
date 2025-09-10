<!DOCTYPE html>

<html lang="en">

<head>

  <meta charset="UTF-8">

  <meta name="viewport" content="width=device-width,initial-scale=1.0">

  <title>Student Portfolio</title>

  <link rel="stylesheet" href="style.css">

  <script defer src="script.js"></script>

  <!-- EmailJS SDK -->

  <script type="text/javascript" src="https://cdn.emailjs.com/dist/email.min.js"></script>

  <script>

    (function(){

      emailjs.init("YOUR_PUBLIC_KEY"); // replace with your EmailJS Public Key

    })();

  </script>

</head>

<body>

  <!-- Navbar -->

  <header>

    <nav class="navbar">

      <div class="logo">MyPortfolio</div>

      <ul class="nav-links" id="nav-links">

        <li><a href="#home">Home</a></li>

        <li><a href="#about">About</a></li>

        <li><a href="#projects">Projects</a></li>

        <li><a href="#contact">Contact</a></li>

      </ul>

      <div class="menu-toggle" id="menu-toggle">&#9776;</div>

    </nav>

  </header>

  <!-- Hero -->

  <section id="home" class="hero">

    <div class="hero-content">

      <h1>Hello, I'm <span>MR__ YOGA</span></h1>

      <p>I am the veti officer</p>

      <a href="#projects" class="btn">View My Work</a>

    </div>

  </section>

  <!-- About -->

  <section id="about" class="about">

    <h2>About Me</h2>

    <div class="about-content">

      <img src="IMG_20250805_154826.jpg" alt="Profile Photo">

      <p>

        I am a student enthusiastic about technology and design. I love building interactive,

        user-friendly web applications and exploring new tools in the tech world.

      </p>

    </div>

  </section>

  <!-- Projects -->

  <section id="projects" class="projects">

    <h2>My Projects</h2>

    <div class="project-grid">

      <div class="project-card">

        <h3>Project 1</h3>

        <p>A simple responsive website.</p>

      </div>

      <div class="project-card">

        <h3>Project 2</h3>

        <p>JavaScript-based quiz app.</p>

      </div>

      <div class="project-card">

        <h3>Project 3</h3>

        <p>Personal blog with CMS.</p>

      </div>

    </div>

  </section>

  <!-- Contact -->

  <section id="contact" class="contact">

    <h2>Contact Me</h2>

    <form id="contact-form">

      <input type="text" id="name" name="user_name" placeholder="Your Name" required>

      <input type="email" id="email" name="user_email" placeholder="Your Email" required>

      <textarea id="message" name="message" placeholder="Your Message" required></textarea>

      <button type="submit">Send</button>

    </form>

    <p id="form-status"></p>

  </section>

  <!-- Footer -->

  <footer>

    <p>&copy; 2025 MR__ YOGA | All rights reserved</p>

  </footer>

</body>

</html>
