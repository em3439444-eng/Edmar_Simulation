<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Edmar Magbanua | Portfolio</title>
  <link rel="stylesheet" href="style.css">
  <style>
    /* Reset and base styles */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
    body { line-height: 1.6; color: #333; background: #f9f9f9; scroll-behavior: smooth; }
    a { text-decoration: none; color: #0077ff; }
    a:hover { text-decoration: underline; }

    /* Header / Nav */
    header { background: #1a1a1a; color: #fff; padding: 1rem 0; position: sticky; top: 0; z-index: 1000; }
    nav { display: flex; justify-content: space-between; align-items: center; width: 90%; margin: auto; }
    nav h1 { font-size: 1.8rem; letter-spacing: 1px; }
    nav ul { list-style: none; display: flex; gap: 2rem; }
    nav ul li a { color: #fff; font-weight: 500; transition: 0.3s; }
    nav ul li a:hover { color: #00d1ff; }

    /* Sections */
    .section { padding: 4rem 1rem; text-align: center; }
    h2 { font-size: 2rem; margin-bottom: 1rem; color: #1a1a1a; }

    /* About */
    .profile { width: 150px; height: 150px; border-radius: 50%; object-fit: cover; margin-bottom: 1rem; border: 3px solid #0077ff; }

    /* Video */
    .video iframe { border-radius: 10px; }

    /* Projects */
    .cards { display: flex; flex-wrap: wrap; justify-content: center; gap: 1.5rem; margin-top: 2rem; }
    .card { background: #fff; padding: 1.5rem; width: 250px; border-radius: 10px; box-shadow: 0 5px 15px rgba(0,0,0,0.1); transition: transform 0.3s, box-shadow 0.3s; }
    .card:hover { transform: translateY(-5px); box-shadow: 0 10px 20px rgba(0,0,0,0.15); }
    .card h3 { margin-bottom: 0.5rem; color: #0077ff; }

    /* Contact */
    #contact a { color: #0077ff; font-weight: 500; }

    /* Footer */
    footer { background: #1a1a1a; color: #fff; padding: 1rem 0; text-align: center; font-size: 0.9rem; }

    /* Responsive */
    @media (max-width: 768px) {
      .cards { flex-direction: column; align-items: center; }
      nav ul { flex-direction: column; gap: 1rem; margin-top: 1rem; }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <nav>
      <h1>Edmar Magbanua</h1>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- About -->
  <section id="about" class="section">
    <img src="/Gemini_Generated_Image_rlrctrlrctrlrctr.png" alt="Edmar Photo" class="profile">
    <h2>Hello, I'm Edmar 👋</h2>
    <p>BSIT Student passionate about web development, UI/UX design, and emerging technologies. I love creating clean and functional digital experiences.</p>
  </section>

  <!-- Video -->
  <section class="section">
    <h2>My Mood 🎬</h2>
    <div class="video">
      <iframe width="100%" height="300" 
        src="https://www.youtube.com/embed/MGRm4IzK1SQ" 
        frameborder="0" allowfullscreen></iframe>
    </div>
  </section>

  <!-- Projects -->
<!-- Projects -->
<section id="projects" class="section">
  <h2>My Projects 💻</h2>
  <div class="cards">
    <div class="card">
      <h3>UI Design Project</h3>
      <p>Crafted sleek user interfaces and prototypes using <a href="https://www.figma.com/proto/DnWfcQfuA3DE6at1UtmNZ9/edmar?node-id=1-2&p=f&t=TYUitMrgVuw9yQu9-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1" target="_blank">Figma</a>.</p>
    </div>
    <div class="card">
      <h3>Graphic Design Project</h3>
      <p>Created engaging graphics and branding assets with <a href="https://www.canva.com/design/your-canva-link" target="_blank">Canva</a>.</p>
    </div>
  </div>
</section>

  <!-- Contact -->
  <section id="contact" class="section">
    <h2>Contact Me 📩</h2>
    <p>Gmail: <a href="magbanuaedmar240@gmail.com:">magbanuaedmar240@gmail.com</a></p>
    <p>Facebook: <a href="https://facebook.com/edmar.pasquil.magbanua" target="_blank">My Profile</a></p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 Edmar Magbanua | All Rights Reserved</p>
  </footer>

</body>
</html>
