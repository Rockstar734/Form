
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Sumit Singh | Portfolio</title>
  <style>
    :root {
      --bg-color: #f9f9f9;
      --text-color: #333;
      --header-bg: #333;
      --header-text: #fff;
      --button-bg: #007BFF;
      --footer-bg: #222;
      --footer-text: #ccc;
    }
    body.dark {
      --bg-color: #121212;
      --text-color: #eee;
      --header-bg: #1f1f1f;
      --header-text: #fff;
      --button-bg: #1e90ff;
      --footer-bg: #000;
      --footer-text: #888;
    }
    body {
      font-family: 'Segoe UI', sans-serif;
      line-height: 1.6;
      background: var(--bg-color);
      color: var(--text-color);
      transition: background 0.3s, color 0.3s;
    }
    .container {
      max-width: 900px;
      margin: auto;
      padding: 20px;
    }
    header {
      background: var(--header-bg);
      color: var(--header-text);
      padding: 60px 0;
      text-align: center;
    }
    header h1 { font-size: 2.5rem; }
    header p { font-size: 1.2rem; color: #ccc; }
    .toggle-btn {
      margin-top: 10px;
      background: var(--button-bg);
      color: white;
      padding: 8px 16px;
      border: none;
      cursor: pointer;
      border-radius: 5px;
    }
    section { margin-top: 40px; }
    h2 { margin-bottom: 20px; }
    .project, .gallery img {
      background: white;
      padding: 15px;
      border: 1px solid #ddd;
      margin-bottom: 20px;
      border-radius: 8px;
      animation: fadeIn 1s ease-in-out;
    }
    .project a {
      color: var(--button-bg);
      text-decoration: none;
    }
    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    form button {
      background: var(--button-bg);
      color: #fff;
      border: none;
      padding: 12px 20px;
      cursor: pointer;
      border-radius: 5px;
    }
    footer {
      text-align: center;
      padding: 20px;
      background: var(--footer-bg);
      color: var(--footer-text);
      margin-top: 40px;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
    }
    .gallery img {
      width: 100%;
      border-radius: 10px;
      transition: transform 0.3s;
    }
    .gallery img:hover {
      transform: scale(1.05);
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <header>
    <div class="container">
      <h1>Sumit Singh</h1>
      <p>Web Developer | Designer | Freelancer</p>
      <button class="toggle-btn" onclick="toggleDarkMode()">Toggle Dark Mode</button>
    </div>
  </header>

  <section id="about" class="container">
    <h2>About Me</h2>
    <p>Hello! I'm Sumit Singh, a passionate web developer with experience in creating modern, responsive websites and applications.</p>
  </section>

  <section id="projects" class="container">
    <h2>Projects</h2>
    <div class="project">
      <h3>Portfolio Website</h3>
      <p>A personal portfolio website showcasing my skills and projects.</p>
      <a href="#">View Project</a>
    </div>
    <div class="project">
      <h3>Todo App</h3>
      <p>A simple and interactive to-do list built with JavaScript.</p>
      <a href="#">View Project</a>
    </div>
  </section>

  <section id="gallery" class="container">
    <h2>Image Gallery</h2>
    <div class="gallery">
      <img src="https://via.placeholder.com/400x300" alt="Project Screenshot 1">
      <img src="https://via.placeholder.com/400x300" alt="Project Screenshot 2">
      <img src="https://via.placeholder.com/400x300" alt="Project Screenshot 3">
    </div>
  </section>

  <section id="resume" class="container">
    <h2>Resume</h2>
    <p>You can download my resume using the button below:</p>
    <a href="https://example.com/Sumit_Singh_Resume.pdf" download class="toggle-btn" style="display:inline-block;margin-top:10px;">Download Resume</a>
  </section>

  <section id="contact" class="container">
    <h2>Contact</h2>
    <h1>FormSubmit Demo</h1>
    <form target="_blank" action="https://formsubmit.co/sumitsinghjh6615@gmail.com" method="POST">
      <input type="hidden" name="_next" value="thank-you.html">
      <input type="hidden" name="_captcha" value="false">
      <div class="form-group">
        <div class="form-row" style="display: flex; gap: 10px; flex-wrap: wrap;">
          <div class="col" style="flex: 1;">
            <input type="text" name="name" class="form-control" placeholder="Full Name" required style="width: 100%; padding: 10px;">
          </div>
          <div class="col" style="flex: 1;">
            <input type="email" name="email" class="form-control" placeholder="Email Address" required style="width: 100%; padding: 10px;">
          </div>
        </div>
      </div>
      <div class="form-group" style="margin-top: 10px;">
        <textarea placeholder="Your Message" class="form-control" name="message" rows="10" required style="width: 100%; padding: 10px;"></textarea>
      </div>
      <button type="submit" class="btn btn-lg btn-dark btn-block" style="margin-top: 10px; padding: 10px 20px; background: #000; color: white; border: none; border-radius: 5px;">Submit Form</button>
    </form>
  </section>

  <footer>
    <div class="container">
      <p>&copy; 2025 Sumit Singh. All rights reserved.</p>
    </div>
  </footer>

  <script>
    function toggleDarkMode() {
      document.body.classList.toggle('dark');
    }
  </script>
</body>
</html>
