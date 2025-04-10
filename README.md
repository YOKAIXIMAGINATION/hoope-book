<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>One Last Time, Love - Launch</title>
  <meta name="description" content="Official launch site for 'One Last Time, Love' by Hoope. Discover the story, follow the countdown, and learn more about the upcoming release on Amazon.">
  <meta property="og:title" content="One Last Time, Love - Book Launch">
  <meta property="og:description" content="Discover the story of Vincent – a tale of love, self-discovery, and redemption. Coming soon to Amazon.">
  <meta property="og:image" content="capa.jpg">
  <meta property="og:type" content="website">
  <meta property="og:url" content="https://your-site-url.com">
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #ffc8e2, #eacdf4, #d4c7f9, #c4d4fc, #c2ebfe);
      background-attachment: fixed;
      overflow-x: hidden;
      position: relative;
      color: white;
    }

    .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 30, 0.1);
      z-index: 0;
    }

    .stars {
      position: absolute;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      z-index: 1;
      pointer-events: none;
    }

    .star {
      position: absolute;
      background: white;
      border-radius: 50%;
      opacity: 0.8;
      animation: twinkle 2s infinite ease-in-out;
    }

    @keyframes twinkle {
      0%, 100% { opacity: 0.8; transform: scale(1); }
      50% { opacity: 0.3; transform: scale(1.2); }
    }

    .bloom {
      position: absolute;
      background: white;
      border-radius: 50%;
      opacity: 0.15;
      filter: blur(12px);
    }

    header {
      position: relative;
      z-index: 2;
      text-align: center;
      padding: 40px 20px 20px 20px;
    }

    .countdown {
      font-size: 2rem;
      font-weight: bold;
      margin-bottom: 20px;
    }

    header img {
      width: 100%;
      max-width: 600px;
      height: auto;
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    }

    .info {
      margin-top: 30px;
      font-size: 1.5rem;
    }

    .quote, .description, .synopsis, .about-author, .coming-soon, .credits, .footer {
      margin-top: 40px;
      font-size: 1.2rem;
      max-width: 700px;
      margin-left: auto;
      margin-right: auto;
      color: white;
    }

    .quote, .description, .synopsis, .about-author, .coming-soon, .credits, .footer {
      border-top: 1px solid rgba(255, 255, 255, 0.4);
      padding-top: 20px;
    }

    .quote {
      font-style: italic;
    }

    .fixed-quote {
      position: fixed;
      top: 55%;
      left: 30px;
      transform: translateY(-50%);
      font-size: 0.95rem;
      font-weight: 300;
      color: white;
      font-family: Arial, sans-serif;
      line-height: 1.6;
      max-width: 350px;
      z-index: 10;
      opacity: 0;
      animation: fadeIn 2.5s ease-in-out forwards;
      pointer-events: none;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .credits-container {
      display: flex;
      justify-content: space-between;
      margin-top: 20px;
      flex-wrap: wrap;
    }

    .credits-container .left, .credits-container .right {
      flex: 1 1 100%;
      padding: 10px;
      text-align: center;
    }

    .footer {
      text-align: center;
      font-size: 0.9rem;
      margin-top: 60px;
      padding-bottom: 40px;
    }

    @media (min-width: 768px) {
      .credits-container .left, .credits-container .right {
        flex: 1;
        text-align: left;
      }
    }

    @media (max-width: 768px) {
      .fixed-quote {
        position: static;
        transform: none;
        margin: 20px auto;
        text-align: center;
        animation: none;
        opacity: 1;
      }

      .countdown {
        font-size: 1.3rem;
      }

      .info {
        font-size: 1.2rem;
      }

      .quote, .description, .synopsis {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>
  <div class="overlay"></div>
  <div class="stars">
    <script>
      for (let i = 0; i < 150; i++) {
        const star = document.createElement('div');
        star.classList.add('star');
        const size = Math.random() * 2 + 1;
        star.style.width = `${size}px`;
        star.style.height = `${size}px`;
        star.style.top = `${Math.random() * 100}%`;
        star.style.left = `${Math.random() * 100}%`;
        document.querySelector('.stars').appendChild(star);
      }

      for (let i = 0; i < 20; i++) {
        const bloom = document.createElement('div');
        bloom.classList.add('bloom');
        const size = Math.random() * 80 + 30;
        bloom.style.width = `${size}px`;
        bloom.style.height = `${size}px`;
        bloom.style.top = `${Math.random() * 100}%`;
        bloom.style.left = `${Math.random() * 100}%`;
        document.querySelector('.stars').appendChild(bloom);
      }
    </script>
  </div>
  <header>
    <div class="fixed-quote">
      Once, Vincent stood by a distant lake and pondered, "If my love were as vast as every drop in this river, how long would it take to run dry?" In that quiet moment, he reached into his pocket, took out a ring, and tossed it into the water, whispering, "Probably faster than I'll ever have the answer."
    </div>
    <div class="countdown" id="countdown"></div>
    <img src="capa.jpg" alt="Book Cover">
    <div class="info">
      <p><strong>Pre-order:</strong> June 20, 2025</p>
      <p><strong>Release Date:</strong> July 20, 2025</p>
      <div class="quote">
        If all my love were just a representation of a vast ocean, would there be anyone I could trust it with? – hoope.
      </div>
      <div class="description">
        <p><strong>En-Us:</strong> Welcome! I'm learning English, and to help with that, I’m launching my first book entirely in English. It’s part of my journey to improve my writing and language skills. Even though this started as a study project, I’m putting my heart into it so it becomes something that anyone can enjoy and connect with. I hope it turns into a book people truly love. Thank you so much to everyone supporting this project!</p>
        <br>
        <p><strong>Pt-Br:</strong> Bem-vindos! Estou aprendendo inglês e, para isso, estou lançando meu primeiro livro inteiramente no idioma. É parte da minha jornada para melhorar minha escrita e compreensão. Mesmo sendo um projeto de estudo, estou colocando todo o meu coração nele, para que se torne algo que qualquer pessoa possa gostar e se identificar. Espero que se torne um livro que as pessoas realmente amem. Muito obrigado a todos que estão apoiando esse projeto!</p>
      </div>
      <div class="synopsis">
        <p><strong>Synopsis:</strong> Vincent has recently been going through internal conflicts. Is he capable of loving or being loved? Is he ready for this feeling? After being rejected by people he trusted, Vincent begins to question what love is and if he has ever truly felt it. This is a story about love, self-discovery, perseverance and redemption.</p>
        <br>
        <p><strong>Sinopse:</strong> Vincent tem passado por conflitos internos ultimamente. Será que ele é capaz de amar ou ser amado? Estará ele pronto para esse sentimento? Após ser rejeitado por pessoas em quem confiava, Vincent começa a questionar o que é o amor e se ele realmente o sentiu. Esta é uma história sobre amor, autodescoberta, perseverança e redenção.</p>
      </div>
    </div>
    <div class="coming-soon">
      <p><strong>Coming soon to Amazon.</strong></p>
    </div>
    <div class="credits">
      <div class="credits-container">
        <div class="left">
          <strong>Patrocinadores/Sponsors:</strong>
          <p>Nenhum por enquanto.</p>
        </div>
        <div class="right">
          <strong>Editora/Publisher:</strong>
          <p style="text-align:center">Nenhuma</p>
        </div>
      </div>
    </div>
    <div class="footer">
      <p><strong>Instagram:</strong> <a href="https://www.instagram.com/_hoopeh_/" style="color:white">Hoope</a> &nbsp;|&nbsp; <strong>Email:</strong> <a href="mailto:Vagante345@gmail.com" style="color:white">Vagante345@gmail.com</a></p>
      <p><strong>Author:</strong> Hoope is a young Brazilian writer passionate about storytelling. Writing has become not only a way to learn English but also a path of self-expression, where emotions, memories, and dreams turn into stories. With "One Last Time, Love," Hoope invites readers on a heartfelt journey of self-discovery and affection.</p>
    </div>
  </header>

  <script>
    const countdown = document.getElementById('countdown');
    const targetDate = new Date("2025-07-20T00:00:00").getTime();

    function updateCountdown() {
      const now = new Date().getTime();
      const distance = targetDate - now;

      if (distance < 0) {
        countdown.innerHTML = "The book has launched!";
        return;
      }

      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((distance % (1000 * 60)) / 1000);

      countdown.innerHTML = `Time until release: ${days}d ${hours}h ${minutes}m ${seconds}s`;
    }

    setInterval(updateCountdown, 1000);
    updateCountdown();
  </script>
</body>
</html>
