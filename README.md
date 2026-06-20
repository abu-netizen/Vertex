<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Trading för nybörjare</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      background: #f1f1f1;
      color: #111;
    }

    .hero {
      min-height: 640px;
      background: #f1f1f1;
      position: relative;
      overflow: hidden;
      display: flex;
      align-items: center;
    }

    .hero::before {
      content: "";
      position: absolute;
      width: 560px;
      height: 360px;
      left: -130px;
      bottom: -190px;
      background: rgba(255, 255, 255, 0.65);
      border-radius: 50%;
    }

    .hero::after {
      content: "";
      position: absolute;
      width: 430px;
      height: 260px;
      right: -40px;
      top: -10px;
      background: rgba(255, 255, 255, 0.6);
      border-radius: 0 0 0 100%;
    }

    .hero-inner {
      width: min(1120px, calc(100% - 48px));
      margin: 0 auto;
      position: relative;
      z-index: 2;
      display: grid;
      grid-template-columns: 1.05fr 0.95fr;
      gap: 56px;
      align-items: center;
    }

    .hero-copy {
      text-align: center;
      max-width: 610px;
      justify-self: center;
    }

    .hero-copy h1 {
      margin: 0 0 30px;
      font-size: clamp(3.1rem, 6vw, 4.8rem);
      line-height: 1.03;
      letter-spacing: -2.2px;
      font-weight: 900;
      color: #050505;
    }

    .hero-copy p {
      margin: 0 auto 34px;
      max-width: 560px;
      color: #111;
      font-size: 1.18rem;
      line-height: 1.48;
    }

    .hero-button {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      min-width: 335px;
      min-height: 68px;
      padding: 18px 34px;
      border-radius: 999px;
      background: #0b7d46;
      color: #fff;
      font-weight: 900;
      font-size: 1rem;
      text-transform: uppercase;
      text-decoration: none;
      letter-spacing: 0.2px;
    }

    .hero-book {
      position: relative;
      display: grid;
      place-items: center;
    }

    .hero-book::before {
      content: "";
      position: absolute;
      width: 260px;
      height: 260px;
      right: 54px;
      bottom: 26px;
      border-radius: 50%;
      background: radial-gradient(
        circle,
        rgba(0, 0, 0, 0.18),
        rgba(0, 0, 0, 0.06) 48%,
        rgba(0, 0, 0, 0) 72%
      );
      filter: blur(12px);
    }

    .hero-book img {
      position: relative;
      z-index: 1;
      width: min(340px, 100%);
      height: auto;
      display: block;
      filter: drop-shadow(0 22px 34px rgba(0, 0, 0, 0.22));
    }

    @media (max-width: 900px) {
      .hero {
        padding: 56px 0;
      }

      .hero-inner {
        grid-template-columns: 1fr;
        text-align: center;
      }

      .hero-book {
        margin-top: 20px;
      }
    }

    @media (max-width: 620px) {
      .hero-copy h1 {
        font-size: 2.8rem;
        letter-spacing: -1.2px;
      }

      .hero-copy p {
        font-size: 1rem;
      }

      .hero-button {
        min-width: 0;
        width: 100%;
      }

      .hero-book img {
        width: min(290px, 92vw);
      }
    }
  </style>
</head>

<body>

  <section class="hero">
    <div class="hero-inner">

      <div class="hero-copy">
        <h1>Trading har äntligen<br>blivit enkelt</h1>

        <p>
          Behärska principerna som 95% av nya traders aldrig lär sig,
          så att du snabbt kan bygga en extra inkomstström.
        </p>

        <a href="#download" class="hero-button">
          Ladda ner gratis guiden
        </a>
      </div>

      <div class="hero-book">
        <img src="assets/guide-cover.png" alt="Handel för nybörjare guidebok">
      </div>

    </div>
  </section>

</body>
</html>
