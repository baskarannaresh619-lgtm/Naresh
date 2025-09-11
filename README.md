<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Student Portfolio - Naresh</title>
  <style>
    /* === Base Styles === */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f9f9f9;
      color: #333;
    }
    header, section, footer {
      padding: 20px;
    }
    a { text-decoration: none; color: inherit; }

    /* Navbar */
    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: #333;
      padding: 15px 20px;
      color: white;
    }
    .nav-links {
      display: flex;
      gap: 15px;
      list-style: none;
    }
    .nav-links a { color: white; font-weight: bold; }
    .menu-toggle { display: none; cursor: pointer; }

    /* Hero */
    .hero {
      background: #eee;
      text-align: center;
      padding: 60px 20px;
    }
    .hero h1 span { color: #007bff; }
    .btn {
      display: inline-block;
      margin-top: 15px;
      padding: 10px 20px;
      background: #007bff;
      color: white;
      border-radius: 5px;
    }

    /* About */
    .about-content {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      align-items: center;
    }
    .about-content img {
      max-width: 200px;
      border-radius: 8px;
    }

    /* Projects */
    .project-grid {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }
    .project-card {
      background: white;
      padding: 15px;
      border-radius: 8px;
      flex: 1;
      min-width: 200px;
      box-shadow: 0 0 5px rgba(0,0,0,0.1);
    }

    /* Contact */
    form {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }
    input, textarea {
      padding: 10px;
      font-size: 16px;
    }
    button {
      padding: 10px;
      background: #007bff;
      color: white;
      border: none;
      border-radius: 5px;
    }

    /* Quiz */
    .quiz-container {
      background-color: white;
      padding: 20px;
      border-radius: 8px;
      max-width: 700px;
      margin: auto;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    .quiz-container h1 { text-align: center; color: #007bff; }
    .question { margin-bottom: 20px; }
    .question pre {
      background: #eee;
      padding: 10px;
      border-radius: 5px;
      overflow-x: auto;
    }
    .options label {
      display: block;
      margin: 5px 0;
      padding: 8px;
      border: 1px solid #ccc;
      border-radius: 5px;
      cursor: pointer;
    }
    #result {
      text-align: center;
      font-weight: bold;
      margin-top: 15px;
    }

    /* Blog */
    .post {
      background: white;
      padding: 15px;
      margin-bottom: 20px;
      border-radius: 8px;
      box-shadow: 0 0 5px rgba(0,0,0,0.1);
    }
    .post h2 { margin: 0 0 10px; }
    .post small { color: gray; font-size: 12px; }

    /* Responsive Nav */
    @media (max-width: 768px) {
      .nav-links { display: none; flex-direction: column; background: #333; }
      .nav-links.active { display: flex; }
      .menu-toggle { display: block; }
    }
  </style>
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
        <li><a href="#quiz">Quiz</a></li>
        <li><a href="#blog">Blog</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
      <div class="menu-toggle" id="menu-toggle">&#9776;</div>
    </nav>
  </header>

  <!-- Hero -->
  <section id="home" class="hero">
    <div class="hero-content">
      <h1>Hello, I'm <span>MR__NARESH</span></h1>
      <p>I am the student</p>
      <a href="#projects" class="btn">View My Work</a>
    </div>
  </section>

  <!-- About -->
  <section id="about" class="about">
    <h2>About Me</h2>
    <div class="about-content">
      <img src="IMG-20250910-WA0007.jpg" alt="Profile Photo">
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
      <div class="project-card"><h3>Project 1</h3><p>A simple responsive website.</p></div>
      <div class="project-card"><h3>Project 2</h3><p>JavaScript-based quiz app.</p></div>
      <div class="project-card"><h3>Project 3</h3><p>Personal blog with CMS.</p></div>
    </div>
  </section>

  <!-- Quiz -->
  <section id="quiz" class="quiz">
    <div class="quiz-container">
      <h1>HTML Quiz</h1>
      <form id="quizForm">

        <!-- Question 1 -->
        <div class="question">
          <h2>1. What will render inside the &lt;h1&gt;?</h2>
          <pre>&lt;h1&gt;Welcome &amp;amp; Hello&lt;/h1&gt;</pre>
          <div class="options">
            <label><input type="radio" name="q1" value="A"> A. Welcome & Hello</label>
            <label><input type="radio" name="q1" value="B"> B. Welcome &amp; Hello</label>
            <label><input type="radio" name="q1" value="C"> C. Welcome < Hello</label>
            <label><input type="radio" name="q1" value="D"> D. nothing — entities don't render</label>
          </div>
        </div>

        <!-- Question 2 -->
        <div class="question">
          <h2>2. If the email field is empty, what happens?</h2>
          <pre>
&lt;form&gt;
  &lt;input type="text" name="name" required&gt;
  &lt;input type="email" name="email" required&gt;
  &lt;button&gt;Send&lt;/button&gt;
&lt;/form&gt;
          </pre>
          <div class="options">
            <label><input type="radio" name="q2" value="A"> A. Form submits with empty email</label>
            <label><input type="radio" name="q2" value="B"> B. Browser shows validation error</label>
            <label><input type="radio" name="q2" value="C"> C. Only name field is sent</label>
            <label><input type="radio" name="q2" value="D"> D. Page reloads with no request</label>
          </div>
        </div>

        <!-- Question 3 -->
        <div class="question">
          <h2>3. Which is true about this &lt;img&gt; tag?</h2>
          <pre>&lt;img src="photo.jpg" alt="Young student" width="600" height="400"&gt;</pre>
          <div class="options">
            <label><input type="radio" name="q3" value="A"> A. alt is optional, only for SEO</label>
            <label><input type="radio" name="q3" value="B"> B. width & height always force size</label>
            <label><input type="radio" name="q3" value="C"> C. alt gives text for accessibility / fallback</label>
            <label><input type="radio" name="q3" value="D"> D. Invalid — width & height must be CSS only</label>
          </div>
        </div>

        <button type="submit">Submit Quiz</button>
      </form>
      <p id="result"></p>
    </div>
  </section>

  <!-- Blog -->
  <section id="blog" class="blog">
    <h2>My Blog</h2>
    <div id="postsContainer"></div>
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
    <p>&copy; 2025 MR__NARESH | All rights reserved</p>
  </footer>

  <script>
    // Navbar toggle
    document.getElementById("menu-toggle").addEventListener("click", function() {
      document.getElementById("nav-links").classList.toggle("active");
    });

    // Quiz logic
    document.getElementById("quizForm").addEventListener("submit", function(e) {
      e.preventDefault();
      let score = 0;
      const answers = { q1: "A", q2: "B", q3: "C" };
      Object.keys(answers).forEach(q => {
        const selected = document.querySelector(\`input[name="\${q}"]:checked\`);
        if (selected && selected.value === answers[q]) { score++; }
      });
      document.getElementById("result").innerText =
        \`You scored \${score} out of \${Object.keys(answers).length}\`;
    });

    // Blog loading
    function loadPosts() {
      const postsContainer = document.getElementById("postsContainer");
      const posts = JSON.parse(localStorage.getItem("blogPosts")) || [
        { title: "My First Post", content: "This is an example blog post.", date: new Date() }
      ];
      postsContainer.innerHTML = "";
      posts.reverse().forEach(post => {
        const postEl = document.createElement("div");
        postEl.classList.add("post");
        postEl.innerHTML = \`
          <h2>\${post.title}</h2>
          <small>\${new Date(post.date).toLocaleString()}</small>
          <p>\${post.content}</p>
        \`;
        postsContainer.appendChild(postEl);
      });
    }
    loadPosts();
  </script>
</body>
</html>
