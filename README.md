<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Abinaya S | Portfolio</title>
  <link rel="icon" href="https://avatars.githubusercontent.com/u/186363000?s=32&v=4" type="image/png" />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }
    body {
      background: linear-gradient(120deg, #fdfbfb, #ebedee);
      color: #333;
      overflow-x: hidden;
    }
    header {
      background-color: #5f27cd;
      color: white;
      padding: 60px 20px;
      text-align: center;
      animation: fadeScale 1.2s ease-in-out;
    }
    header h1 {
      font-size: 2.8rem;
      animation: fadeIn 1.2s ease-in-out;
    }
    .typing {
      font-size: 1.2rem;
      margin-top: 10px;
      border-right: 2px solid white;
      white-space: nowrap;
      overflow: hidden;
      display: inline-block;
      animation: typing 3s steps(30, end) forwards, blink 0.8s infinite;
      max-width: 100%;
    }
    .profile-img {
      width: 140px;
      height: 140px;
      border-radius: 50%;
      margin-top: 20px;
      object-fit: cover;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      border: 4px solid white;
      transition: transform 0.4s ease;
      animation: zoomIn 1s ease;
    }
    .profile-img:hover {
      transform: scale(1.08);
    }
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 1s ease, transform 1s ease;
    }
    section.visible {
      opacity: 1;
      transform: translateY(0);
    }
    h2 {
      font-size: 2rem;
      color: #5f27cd;
      margin-bottom: 20px;
      animation: fadeIn 1.2s ease-in-out;
    }
    .skills, .projects {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
    }
    .skill, .project {
      flex: 1 1 45%;
      background-color: #fff;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.05);
      transition: transform 0.4s ease, box-shadow 0.4s ease;
      opacity: 0;
      transform: translateY(20px);
      animation: slideIn 0.8s forwards;
    }
    .skill:hover, .project:hover {
      transform: scale(1.05);
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);
    }
    .project h3 {
      margin-bottom: 10px;
    }
    .contact a {
      display: inline-block;
      margin: 10px 10px 0 0;
      text-decoration: none;
      color: #5f27cd;
      font-weight: 600;
      transition: transform 0.3s;
      animation: fadeIn 1s ease;
    }
    .contact a:hover {
      transform: scale(1.05);
    }
    footer {
      text-align: center;
      padding: 30px 20px;
      background-color: #333;
      color: white;
      animation: fadeUp 1.2s ease-in-out;
    }

    @keyframes fadeScale {
      from { opacity: 0; transform: scale(0.9); }
      to { opacity: 1; transform: scale(1); }
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes zoomIn {
      from { transform: scale(0.8); opacity: 0; }
      to { transform: scale(1); opacity: 1; }
    }

    @keyframes slideIn {
      from { transform: translateY(40px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink {
      50% { border-color: transparent; }
    }

    @media (max-width: 600px) {
      .skill, .project {
        flex: 1 1 100%;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Abinaya S</h1>
    <img src="https://avatars.githubusercontent.com/u/186363000?s=96&v=4" alt="Profile image of Abinaya S" class="profile-img" />
    <p class="typing">Aspiring Software Developer | Tech Explorer</p>
  </header>

  <section id="about">
    <h2>About Me</h2>
    <p>I am currently pursuing B.E in Computer Science and Engineering at Sri Ramakrishna Engineering College, Coimbatore. I am passionate about exploring Artificial Intelligence, Full Stack Development and building software that solves real-world problems. I'm currently learning C, C++, Python, and Web Development.</p>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <div class="skills">
      <div class="skill" style="animation-delay: 0s;">C</div>
      <div class="skill" style="animation-delay: 0.1s;">C++</div>
      <div class="skill" style="animation-delay: 0.2s;">Python</div>
    </div>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="projects">
      <div class="project" style="animation-delay: 0.2s;">
        <h3>Portfolio Website</h3>
        <p>This website you’re viewing! Built with HTML, CSS, and JavaScript to showcase my skills and passion for web development.</p>
      </div>
      <div class="project" style="animation-delay: 0.4s;">
        <h3>Student Result System</h3>
        <p>A CLI-based result management system built in Python to manage and display academic performance efficiently.</p>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <div class="contact">
      <a href="mailto:abinayatech.dev@gmail.com">📧 abinayatech.dev@gmail.com</a>
      <a href="https://github.com/abinayatech" target="_blank">💻 GitHub</a>
      <a href="https://www.linkedin.com/in/abinaya-saravanan-3a601a328" target="_blank">🔗 LinkedIn</a>
    </div>
  </section>

  <footer>
    <p>© 2025 Abinaya S. Built with 💜 and code.</p>
  </footer>

  <script>
    const sections = document.querySelectorAll('section');
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
        }
      });
    }, {
      threshold: 0.1
    });

    sections.forEach(section => observer.observe(section));
  </script>
</body>
</html>
