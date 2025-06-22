<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Max Kellady | Portfolio</title>
  <style>
    body {
      font-family: 'Poppins', Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #537aa8, #6c8ebf);
      color: #000;
      line-height: 1.6;
      min-height: 100vh;
    }

    .container {
      background: #fff;
      border-radius: 12px;
      padding: 2rem 2.5rem;
      max-width: 800px;
      margin: 2rem auto;
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
    }

    header {
      text-align: center;
      background: none;
      padding: 0;
      margin-bottom: 2rem;
    }

    header .header-content {
      background: #fff;
      border-radius: 12px;
      padding: 2rem 2.5rem;
      max-width: 800px;
      margin: 0 auto 2rem auto;
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
      color: #000;
    }

    header h1 {
      margin: 0 0 0.5rem 0;
      font-size: 2.5rem;
      letter-spacing: 1.5px;
    }

    header h2 {
      margin: 0;
      font-size: 1.2rem;
      font-weight: normal;
      color: #444;
    }

    #about-me h2 {
      margin-top: 0;
      font-size: 1.6rem;
      font-weight: bold;
      color: #000;
      border-bottom: 2px solid #ddd;
      padding-bottom: 0.3rem;
    }

    #about-me p {
      margin: 1rem 0 0 0;
      font-size: 1rem;
      color: #000;
      white-space: pre-line;
    }

    .email {
      color: #1a73e8;
      font-weight: 500;
    }

    details {
      background: #fff;
      border-radius: 12px;
      margin: 1rem 0;
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
      color: #000;
      padding: 0;
    }

    summary {
      font-size: 1.2rem;
      font-weight: bold;
      cursor: pointer;
      position: relative;
      padding: 1.5rem 2rem;
      user-select: none;
      outline: none;
    }

    summary::before {
      content: "▶";
      position: absolute;
      left: 1rem;
      top: 50%;
      transform: translateY(-50%);
      transition: transform 0.3s ease;
    }

    details[open] summary::before {
      transform: translateY(-50%) rotate(90deg);
    }

    .content {
      overflow: hidden;
      max-height: 0;
      opacity: 0;
      padding: 0 2rem;
      transition: max-height 0.5s ease, opacity 0.5s ease, padding 0.5s ease;
    }

    details[open] .content {
      max-height: 2000px;
      opacity: 1;
      padding: 1rem 2rem 2rem 2rem;
    }

    ul {
      list-style: disc inside;
      padding-left: 1.2rem;
      margin-top: 0.5rem;
    }

    li {
      padding: 0.3rem 0;
    }

    summary::-webkit-details-marker,
    summary::marker {
      display: none;
    }

    a {
      color: #2a5298;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    a:hover {
      color: #1e3c72;
      text-decoration: underline;
    }

    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 12px;
    }

    .thumbnail {
      width: 150px;
      cursor: pointer;
      border-radius: 6px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }

    .lightbox {
      display: none;
      position: fixed;
      z-index: 999;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0, 0, 0, 0.9);
      justify-content: center;
      align-items: center;
      flex-direction: column;
    }

    .lightbox img {
      max-width: 90%;
      max-height: 80%;
      border-radius: 8px;
    }

    .lightbox .caption {
      margin-top: 1rem;
      color: #fff;
      font-size: 1rem;
    }

    .lightbox .nav {
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
      font-size: 2rem;
      color: white;
      background: rgba(0, 0, 0, 0.4);
      border: none;
      cursor: pointer;
      padding: 0.5rem 1rem;
      z-index: 1001;
    }

    .lightbox .prev {
      left: 10px;
    }

    .lightbox .next {
      right: 10px;
    }

    .lightbox .close {
      position: absolute;
      top: 20px;
      right: 30px;
      font-size: 2rem;
      color: white;
      cursor: pointer;
    }

    @media (hover: none) {
      .lightbox img {
        max-width: 95%;
        max-height: 75%;
      }
    }
  </style>
</head>
<body>

  <header>
    <div class="header-content">
      <h1>My EAE Portfolio</h1>
      <h2>Aspiring and passionate engineering and technology student</h2>
    </div>
  </header>

  <section id="about-me" class="container">
    <h2>About Me</h2>
    <p>
      Max Kellady

      <br><br>Email (School): <span class="email">max_xavier_kellady@students.edu.sg</span>

      <br><br>Personal Email: <span class="email">shqrked8373@gmail.com</span>

      <br><br>Phone Number: 9175 2848
    </p>
  </section>

  <section class="container">
    <details>
      <summary>Skills & Interests</summary>
      <div class="content">
        <ul>
          <li>Design & Technology</li>
          <li>Engineering</li>
          <li>DIY Crafting (e.g., Woodworking)</li>
          <li>Dancing</li>
          <li>Acting</li>
          <li>3D Printing</li>
        </ul>
      </div>
    </details>

    <details>
      <summary>School Projects</summary>
      <div class="content">
        <ul>
          <li>Wooden Coin Bank</li>
          <li>Custom Improved Torchlight Design</li>
          <li>Key/Coin Holder</li>
          <li>Kite Winder</li>
          <li>Moving Toy Car</li>
          <li>Phone Holder</li>
          <li>O-Levels Project: Display Stand for Funko Pop</li>
          <li>President of Drama CCA</li>
          <li>Participation in Computer Programming Programme by Edublitz</li>
        </ul>
      </div>
    </details>

    <details>
      <summary>Achievements: Photos</summary>
      <div class="content gallery" id="gallery">
        <!-- Photos removed -->
      </div>
    </details>

    <details>
      <summary>Write ups</summary>
      <div class="content">
        <p>My name is Max Kellady. Ever since I was young, I have been fascinated by how things work, understanding mechanisms and figuring out how to build my own. Whenever opportunities arose, I eagerly took them. In primary school, I participated in the Innovation Programme (IVP) and attended an after-school Microbit coding class. I also explored my interests through several STEM kits at home, which helped me learn the basics of electronics and programming.</p>
        <p>In secondary school, I continued to develop my passion by joining the Computer Programming Programme and the AR/VR Programme. These experiences have deepened my understanding of technology and problem-solving.</p>
        <p>After visiting the Singapore Polytechnic open house, I was impressed by the hands-on projects and innovative work being done in the Mechatronics course. It confirmed my desire to study there because I want to gain practical skills and knowledge that will prepare me for a career combining mechanics, electronics, and software.</p>
        <p>I am excited about the opportunity to learn in an environment where creativity and technology come together, and I am confident that Singapore Polytechnic’s Mechatronics course will help me achieve my future goals.</p>
      </div>
    </details>
  </section>

  <!-- Lightbox HTML (still included for future use) -->
  <div class="lightbox" id="lightbox">
    <span class="close" onclick="closeLightbox()">×</span>
    <button class="nav prev" onclick="changeImage(-1)">❮</button>
    <img id="lightbox-img" src="" alt="">
    <div class="caption" id="lightbox-caption"></div>
    <button class="nav next" onclick="changeImage(1)">❯</button>
  </div>

  <script>
    const lightbox = document.getElementById("lightbox");
    const lightboxImg = document.getElementById("lightbox-img");
    const caption = document.getElementById("lightbox-caption");
    const thumbnails = document.querySelectorAll(".thumbnail");
    let currentIndex = 0;

    thumbnails.forEach((img, index) => {
      img.addEventListener("click", () => {
        showImage(index);
      });
    });

    function showImage(index) {
      const img = thumbnails[index];
      lightboxImg.src = img.src;
      caption.textContent = img.dataset.title;
      lightbox.style.display = "flex";
      currentIndex = index;
    }

    function closeLightbox() {
      lightbox.style.display = "none";
    }

    function changeImage(step) {
      currentIndex = (currentIndex + step + thumbnails.length) % thumbnails.length;
      showImage(currentIndex);
    }

    // Touch swipe support
    let startX = 0;
    lightbox.addEventListener("touchstart", e => startX = e.touches[0].clientX);
    lightbox.addEventListener("touchend", e => {
      let endX = e.changedTouches[0].clientX;
      if (endX < startX - 50) changeImage(1);      // Swipe left
      else if (endX > startX + 50) changeImage(-1); // Swipe right
    });
  </script>
</body>
</html>
