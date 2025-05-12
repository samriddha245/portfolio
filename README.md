<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1" />
<title>Portfolio</title>
<style>
  /* Reset & base */
  *, *::before, *::after {
    box-sizing: border-box;
  }
  body {
    margin: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: #0f2027;  /* fallback for old browsers */
    background: linear-gradient(to right, #2c5364, #203a43, #0f2027);
    color: #eee;
    line-height: 1.6;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
  a {
    color: #00aaff;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  a:hover, a:focus {
    color: #1de9b6;
    outline: none;
  }
  /* Layout */
  .container {
    max-width: 900px;
    margin: 0 auto;
    padding: 0 20px 60px;
  }
  header {
    padding: 40px 0 60px;
    border-bottom: 2px solid #00aaff;
    display: flex;
    align-items: center;
    gap: 30px;
    flex-wrap: wrap;
    justify-content: center;
  }
  header img.profile-photo {
    width: 150px;
    height: 150px;
    object-fit: cover;
    border-radius: 50%;
    box-shadow: 0 0 15px 3px rgba(29, 233, 182, 0.6);
    flex-shrink: 0;
  }
  .header-text {
    max-width: 600px;
    text-align: left;
  }
  header h1 {
    margin: 0;
    font-size: 3rem;
    font-weight: 700;
    letter-spacing: 2px;
    color: #1de9b6;
  }
  header p {
    margin-top: 12px;
    font-size: 1.2rem;
    font-weight: 300;
    font-style: italic;
    color: #d4d4d4;
  }
  nav {
    margin-top: 30px;
    text-align: center;
    width: 100%;
  }
  nav a {
    margin: 0 15px;
    font-weight: 600;
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: 1px;
  }
  /* Section styling */
  section {
    margin-top: 60px;
  }
  section h2 {
    font-size: 2rem;
    border-left: 6px solid #1de9b6;
    padding-left: 12px;
    margin-bottom: 25px;
  }
  /* About */
  #about p {
    font-size: 1.1rem;
    max-width: 700px;
    margin-left: auto;
    margin-right: auto;
  }
  /* Skills */
  #skills ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    list-style: none;
    padding: 0;
    margin: 0 -10px;
  }
  #skills li {
    background: #1de9b6;
    color: #0f2027;
    padding: 8px 18px;
    margin: 8px 10px;
    border-radius: 20px;
    font-weight: 600;
    font-size: 1rem;
    box-shadow: 0 3px 5px rgba(0, 0, 0, 0.2);
    user-select: none;
  }
  /* Projects */
  #projects .project {
    background: #203a43;
    margin-bottom: 25px;
    padding: 20px;
    border-radius: 10px;
    transition: transform 0.3s ease;
  }
  #projects .project:hover, #projects .project:focus-within {
    transform: translateY(-5px);
    box-shadow: 0 12px 20px rgba(29, 233, 182, 0.5);
  }
  #projects .project h3 {
    margin-top: 0;
    color: #1de9b6;
  }
  #projects .project p {
    margin-bottom: 10px;
  }
  #projects .project a {
    display: inline-block;
    font-weight: 700;
    background: #1de9b6;
    color: #0f2027;
    padding: 8px 14px;
    border-radius: 8px;
    transition: background-color 0.3s ease;
  }
  #projects .project a:hover, #projects .project a:focus {
    background: #00aaff;
    outline: none;
  }
  /* Contact */
  #contact form {
    max-width: 400px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
  }
  #contact label {
    margin-bottom: 6px;
    font-weight: 600;
  }
  #contact input, #contact textarea {
    padding: 12px 14px;
    margin-bottom: 18px;
    border: none;
    border-radius: 8px;
    font-size: 1rem;
    font-family: inherit;
    resize: vertical;
  }
  #contact textarea {
    min-height: 100px;
  }
  #contact button {
    background: #1de9b6;
    border: none;
    padding: 14px;
    font-weight: 700;
    font-size: 1.1rem;
    border-radius: 8px;
    color: #0f2027;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  #contact button:hover, #contact button:focus {
    background: #00aaff;
    outline: none;
  }
  /* Footer */
  footer {
    text-align: center;
    padding: 15px 0;
    font-size: 0.9rem;
    color: #777;
    border-top: 1px solid #222c32;
  }
  /* Responsive */
  @media (max-width: 600px) {
    header {
      flex-direction: column;
      text-align: center;
    }
    .header-text {
      max-width: 100%;
      text-align: center;
    }
    nav {
      margin-top: 20px;
    }
    #skills ul {
      justify-content: flex-start;
    }
  }
</style>
</head>
<body>
  <div class="container" role="main">
    <header>
      <div class="header-text">
        <h1>Samriddha Dhakal</h1>
        <p>Web Developer & Designer</p>
      </div>
      <nav>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <section id="about" tabindex="-1">
      <h2>About Me</h2>
      <p>Hello! I'm Your Name, a passionate web developer focused on building clean and modern websites and applications. I enjoy creating responsive, user-friendly interfaces with a touch of beautiful design.</p>
    </section>

    <section id="skills" tabindex="-1">
      <h2>Skills</h2>
      <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JS</li>
        <li>GitHub</li>
        <li>Responsive Design</li>
      </ul>
    </section>

    <section id="projects" tabindex="-1">
      <h2>Projects</h2>
      <article class="project" tabindex="0" aria-label="Project 1: Portfolio Website">
        <h3>Portfolio Website</h3>
        <p>A modern and responsive portfolio website to showcase my work and skills. Built with HTML, CSS, and JavaScript.</p>
        <a href="https://github.com/" target="_blank" rel="noopener noreferrer">View on GitHub</a>
      </article>
      <article class="project" tabindex="0" aria-label="Project 2: Task Manager App">
        <h3>Task Manager App</h3>
        <p>A web app to manage daily tasks with CRUD features and local storage support. Built with React and styled-components.</p>
        <a href="https://github.com/yourusername/task-manager" target="_blank" rel="noopener noreferrer">View on GitHub</a>
      </article>
    </section>

    <section id="contact" tabindex="-1" aria-label="Contact form">
      <h2>Contact Me</h2>
      <form onsubmit="event.preventDefault(); alert('Thank you for your message! I will get back to you soon.')">
        <label for="name">Name</label>
        <input type="text" id="name" name="name" required aria-required="true" />
        
        <label for="email">Email</label>
        <input type="email" id="email" name="email" required aria-required="true" />

        <label for="message">Message</label>
        <textarea id="message" name="message" required aria-required="true"></textarea>

        <button type="submit" aria-label="Send message">Send</button>
      </form>
    </section>
  </div>

  <footer>
    &copy; 2025 All rights reserved.
  </footer>
</body>
</html>
