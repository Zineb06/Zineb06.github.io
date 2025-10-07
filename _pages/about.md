---
permalink: /
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
  body {
    font-family: "Inter", "Segoe UI", Roboto, sans-serif;
    line-height: 1.7;
    margin: 0;
    padding: 0;
  }

  .about-container {
    max-width: 950px !important;
    margin: 3rem auto;
    padding: 2rem;
    border-radius: 16px;
    box-shadow: 0 4px 16px rgba(0, 0, 0, 0.05);
  }

  @media (max-width: 1024px) {
    .about-container {
      margin: 2rem auto;
      max-width: 90%;
    }
  }

  .quote {
    text-align: center;
    font-style: italic;
    font-size: 1.2rem;
    margin-bottom: 1.5rem;
    transition: color 0.3s ease;
  }

  .quote span {
    font-weight: 600;
  }

  .image-container {
    text-align: center;
    margin: 1.5rem 0;
  }

  .image-container img {
    width: 80%;
    max-width: 450px;
    border-radius: 12px;
    box-shadow: 0 6px 14px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
  }

  .image-container img:hover {
    transform: scale(1.03);
  }

  .about-text {
    text-align: justify;
    font-size: 1.05rem;
  }

  .contact {
    text-align: center;
    margin-top: 2rem;
    font-style: italic;
  }

  a {
    color: #007acc;
    text-decoration: none;
  }
</style>

<div class="about-container">
  <p class="quote" id="quote">
    “Simplicity is the ultimate sophistication.” — <span>L. D. Vinci</span>
  </p>

  <div class="image-container">
    <img src="/images/chaos_theory.jpg" alt="Chaos Theory" />
  </div>

  <div class="about-text">
    <p>
      Hello! I am a Software Engineering student, currently in my final year. 
      I hold a Master’s degree in Business Intelligence, where I specialized in data-driven decision-making and analytics.
    </p>

    <p>
      I’m passionate about bridging the gap between technology and business needs,
      with a strong interest in software engineering, backend development, and data analysis.
      My academic and project experience allowed me to work with modern technologies and explore fields like system design and machine learning.
      I am particularly interested in generative AI and how it can transform the way we learn, create, and collaborate.
    </p>

    <p>
      I believe web technologies should serve humanity-making knowledge, collaboration, and opportunities more accessible,
      while improving human decision-making. My interests include software engineering, distributed systems,
      data-driven applications, and the evolving role of AI in building meaningful solutions.
    </p>

    <p>
      Outside of coding, I’m involved in volunteering to create a positive social impact.
      I contribute to the association <a href="https://tousinclus-asso.fr">Tous Inclus</a>, helping to develop a SaaS that promote inclusion
      for people with special needs and the elderly. I'm also a member of the association <a href="https://www.faune-alfort.org">Faune Alfort</a> that is focused on animal saving and well-being.
    </p>

    <p>
      I’m deeply committed to continuous learning and using technology to make a meaningful difference in society.
    </p>

  </div>

  <p class="contact">
    📧 Contact me at <a href="mailto:zineb.houmaidi@etud.univ-evry.fr">zineb.houmaidi@etud.univ-evry.fr</a>
  </p>
</div>

<script>
  const quotes = [
    "“Simplicity is the ultimate sophistication.” — L. D. Vinci",
  ];

  const colors = ["#007acc", "#2c3e50", "#16a085", "#8e44ad", "#c0392b"];
  const quoteElement = document.getElementById("quote");

  quoteElement.addEventListener("mouseenter", () => {
    const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
    const randomColor = colors[Math.floor(Math.random() * colors.length)];
    quoteElement.style.color = randomColor;
    quoteElement.innerHTML = randomQuote;
  });

  quoteElement.addEventListener("mouseleave", () => {
    quoteElement.style.color = "";
    quoteElement.innerHTML = "“Simplicity is the ultimate sophistication.” — <span>L. D. Vinci</span>";
  });
</script>
