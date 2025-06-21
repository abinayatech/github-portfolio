<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Abinaya S | Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet">
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
      animation: fadeDown 1s ease-in-out;
      position: relative;
    }
    header h1 {
      font-size: 2.8rem;
    }
    .typing {
      font-size: 1.2rem;
      margin-top: 10px;
      border-right: 2px solid white;
      white-space: nowrap;
      overflow: hidden;
      width: 0;
      animation: typing 3s steps(40, end) forwards, blink 0.8s infinite;
    }
    .profile-img {
      width: 140px;
      height: 140px;
      border-radius: 50%;
      margin-top: 20px;
      object-fit: cover;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
      border: 4px solid white;
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
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .skill:hover, .project:hover {
      transform: translateY(-5px);
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
    }
    .contact a:hover {
      transform: scale(1.05);
    }
    footer {
      text-align: center;
      padding: 30px 20px;
      background-color: #333;
      color: white;
      animation: fadeUp 1s ease-in-out;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeDown {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
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
  </style>
</head>
<body>
  <header>
    <h1>Abinaya S</h1>
    <img src="https://avatars.githubusercontent.com/u/186363000?s=96&v=4" alt="Abinaya S" class="profile-img" />
    <p class="typing">Aspiring Software Developer | Tech Explorer</p>
  </header>

  <section id="about">
    <h2>About Me</h2>
    <p>I am currently pursuing B.E in Computer Science and Engineering at Sri Ramakrishna Engineering College, Coimbatore. I am passionate about exploring Artificial Intelligence, Full Stack Development and building software that solves real-world problems. I'm currently learning C, C++, Python, and Web Development.</p>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <div class="skills">
      <div class="skill">C</div>
      <div class="skill">C++</div>
      <div class="skill">Python</div>
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
