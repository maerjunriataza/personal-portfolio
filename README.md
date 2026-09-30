<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Personal portfolio of Maerjun P. Riataza, a BSIT student at Caraga State University featuring skills, projects, and contact details.">
  <link rel="stylesheet" href="style.css">
  <title>Maerjun P. Riataza - Portfolio</title>
</head>
<body>

  <header>
    <h1>Maerjun P. Riataza</h1>
    <p>BSIT Student | Caraga State University</p>
    <nav>
      <ul>
        <li><a href="#about">About Me</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>About Me</h2>
      <p>Hi! I am Maer, a 22-year-old BSIT student from Caraga State University - Main Campus who is eager to learn Web Systems and Technology.</p>
    </section>

    <section id="skills">
      <h2>Skills</h2>
      <ul>
        <li>Photography</li>
        <li>Dancing</li>
        <li>Writing</li>
        <li>Grammar Checking</li>
        <li>Visuals</li>
      </ul>
    </section>

    <section id="projects">
      <h2>Projects</h2>
      <article>
        <h3>The Visual</h3>
        <img src="https://via.placeholder.com/400x200" alt="Preview banner for The Visual creative portfolio project">
        <p>A curated showcase combining visual arts, digital photography, and creative design compositions.</p>
        <p><a href="https://github.com" target="_blank" rel="noopener noreferrer">View The Visual on GitHub</a></p>
      </article>
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <p>Email: <a href="mailto:maerjun.riataza@carsu.edu.ph">maerjun.riataza@carsu.edu.ph</a></p>
      <p>GitHub: <a href="https://github.com" target="_blank" rel="noopener noreferrer">Visit My GitHub Profile</a></p>

      <form action="#" method="post">
        <p>
          <label for="full-name">Your Name:</label><br>
          <input type="text" id="full-name" name="full-name" required>
        </p>
        <p>
          <label for="email-address">Your Email:</label><br>
          <input type="email" id="email-address" name="email-address" required>
        </p>
        <p>
          <label for="user-message">Message:</label><br>
          <textarea id="user-message" name="user-message" rows="4" cols="30" required></textarea>
        </p>
        <button type="submit">Send Message</button>
      </form>
    </section>
  </main>

  <footer>
    <p>&copy; 2026 Maerjun P. Riataza. All rights reserved.</p>
  </footer>

</body>
</html>

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

:root {
  --bg-primary: #f8fafc;
  --bg-surface: #ffffff;
  --text-main: #1e293b;
  --text-muted: #475569;
  --accent: #0f766e;
  --accent-hover: #115e59;
  --border-color: #e2e8f0;
  --focus-ring: #0284c7;
}

body {
  font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  line-height: 1.6;
  color: var(--text-main);
  background-color: var(--bg-primary);
  font-size: 1rem;
}

header {
  background-color: var(--bg-surface);
  border-bottom: 1px solid var(--border-color);
  padding: 2.5rem 1.5rem 1.5rem;
  text-align: center;
}

header h1 {
  font-size: 2.25rem;
  color: var(--accent);
  margin-bottom: 0.25rem;
}

header > p {
  color: var(--text-muted);
  font-size: 1.1rem;
  margin-bottom: 1.5rem;
}

nav ul {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 1.5rem;
  list-style: none;
}

nav a {
  text-decoration: none;
  color: var(--text-main);
  font-weight: 600;
  padding: 0.5rem 0.75rem;
  border-radius: 4px;
  transition: color 0.2s ease, background-color 0.2s ease;
}

nav a:hover {
  color: var(--accent);
  background-color: #f1f5f9;
}

main {
  max-width: 850px;
  margin: 2rem auto;
  padding: 0 1.25rem;
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

section {
  background-color: var(--bg-surface);
  border: 1px solid var(--border-color);
  border-radius: 8px;
  padding: 2rem;
}

h2 {
  font-size: 1.6rem;
  color: var(--accent);
  border-bottom: 2px solid var(--border-color);
  padding-bottom: 0.5rem;
  margin-bottom: 1.25rem;
}

#skills ul {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  list-style: none;
}

#skills li {
  background-color: #f0fdfa;
  color: var(--accent);
  border: 1px solid #99f6e4;
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-weight: 500;
}

#projects article {
  border: 1px solid var(--border-color);
  border-radius: 8px;
  padding: 1.5rem;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.05);
  background-color: #ffffff;
}

#projects h3 {
  font-size: 1.3rem;
  margin-bottom: 1rem;
}

#projects img {
  width: 100%;
  max-width: 400px;
  height: auto;
  border-radius: 6px;
  display: block;
  margin-bottom: 1rem;
}

#projects p {
  margin-bottom: 0.75rem;
}

#contact form {
  margin-top: 1.5rem;
  display: flex;
  flex-direction: column;
  gap: 1rem;
  max-width: 500px;
}

label {
  font-weight: 600;
  display: inline-block;
  margin-bottom: 0.25rem;
}

input[type="text"],
input[type="email"],
textarea {
  width: 100%;
  padding: 0.65rem 0.85rem;
  border: 1px solid var(--border-color);
  border-radius: 6px;
  font-family: inherit;
  font-size: 1rem;
  background-color: #fdfdfd;
}

button[type="submit"] {
  align-self: flex-start;
  background-color: var(--accent);
  color: #ffffff;
  border: none;
  padding: 0.75rem 1.75rem;
  font-size: 1rem;
  font-weight: 600;
  border-radius: 6px;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

button[type="submit"]:hover {
  background-color: var(--accent-hover);
}

a {
  color: var(--accent);
}

a:hover {
  color: var(--accent-hover);
}

a:focus-visible,
button:focus-visible,
input:focus-visible,
textarea:focus-visible {
  outline: 3px solid var(--focus-ring);
  outline-offset: 2px;
}

footer {
  text-align: center;
  padding: 2rem 1.25rem;
  color: var(--text-muted);
  border-top: 1px solid var(--border-color);
  background-color: var(--bg-surface);
  margin-top: 2rem;
}

@media (max-width: 600px) {
  header h1 {
    font-size: 1.75rem;
  }

  nav ul {
    gap: 0.75rem;
  }

  section {
    padding: 1.25rem;
  }

  button[type="submit"] {
    width: 100%;
  }
}
