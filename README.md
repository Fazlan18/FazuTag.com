<!DOCTYPE html>
<html lang="en">
  <head>
    <style>
      /* Importing Google font - Open Sans */
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;500;600;700&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Open Sans", sans-serif;
}

body {
  height: 100vh;
  width: 100%;
  background: linear-gradient(to bottom, #175d69 23%, #330c43 95%);
}

.header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
}

.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 15px;
}

.navbar .logo a {
  font-size: 1.8rem;
  text-decoration: none;
  color: #fff;
}

.navbar .links {
  display: flex;
  align-items: center;
  list-style: none;
  gap: 35px;
}

.navbar .links a {
  font-weight: 500;
  text-decoration: none;
  color: #fff;
  padding: 10px 0;
  transition: 0.2s ease;
}

.navbar .links a:hover {
  color: #47b2e4;
}

.navbar .buttons a {
  text-decoration: none;
  color: #fff;
  font-size: 1rem;
  padding: 15px 0;
  transition: 0.2s ease;
}

.navbar .buttons a:not(:last-child) {
  margin-right: 30px;
}

.navbar .buttons .signin:hover {
  color: #47b2e4;
}

.navbar .buttons .signup {
  border: 1px solid #fff;
  padding: 10px 20px;
  border-radius: 0.375rem;
  text-align: center;
  transition: 0.2s ease;
}

.navbar .buttons .signup:hover {
  background-color: #47b2e4;
  color: #fff;
}

.hero-section {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  height: 95vh;
  padding: 0 15px;
  max-width: 1200px;
  margin: 0 auto;
}

.hero-section .hero {
  max-width: 50%;
  color: #fff;
}

.hero h2 {
  font-size: 2.5rem;
  margin-bottom: 20px;
}

.hero p {
  font-size: 1.2rem;
  margin-bottom: 20px;
  color: #c9c7c7;
}

.hero-section .img img {
  width: 517px;
}

.hero-section .buttons {
  margin-top: 40px;
}

.hero-section .buttons a {
  text-decoration: none;
  color: #fff;
  padding: 12px 24px;
  border-radius: 0.375rem;
  font-weight: 600;
  transition: 0.2s ease;
  display: inline-block;
}

.hero-section .buttons a:not(:last-child) {
  margin-right: 15px;
}

.buttons .join {
  background-color: #47b2e4;
}

.hero-section .buttons .learn {
  border: 1px solid #fff;
  border-radius: 0.375rem;
}

.hero-section .buttons a:hover {
  background-color: #47b2e4;
}

/* Hamburger menu styles */
#menu-toggle {
  display: none;
}

#hamburger-btn {
  font-size: 1.8rem;
  color: #fff;
  cursor: pointer;
  display: none;
  order: 1;
}

@media screen and (max-width: 1023px) {
  .navbar .logo a {
    font-size: 1.5rem;
  }

  .links {
    position: fixed;
    left: -100%;
    top: 75px;
    width: 100%;
    height: 100vh;
    padding-top: 50px;
    background: #175d69;
    flex-direction: column;
    transition: 0.3s ease;
  }

  .navbar #menu-toggle:checked ~ .links {
    left: 0;
  }

  .navbar #hamburger-btn {
    display: block;
  }

  .header .buttons {
    display: none;
  }

  .hero-section .hero {
    max-width: 100%;
    text-align: center;
  }

  .hero-section img {
    display: none;
  }
}
    </style>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Fazlan</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <header class="header">
      <nav class="navbar">
        <h2 class="logo"><a href="#">Fazlan</a></h2>
        <input type="checkbox" id="menu-toggle" />
        <label for="menu-toggle" id="hamburger-btn">
          <svg xmlns="http://www.w3.org/2000/svg" height="24" viewBox="0 0 24 24" width="24">
            <path d="M3 12h18M3 6h18M3 18h18" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </label>
        <ul class="links">
          <li><a href="Faz.html">Home</a></li>
          <li><a href="About.html">About Us</a></li>
          <li><a href="Gallery.html">Gallery</a></li>
          <li><a href="Editz.html">Editz</a></li>
          <li><a href="Service.html">Services</a></li>
          <li><a href="BLOG.html">BLOG</a></li>
        </ul>
        <div class="buttons">
          <a href="sign in.html" class="signin">Sign In</a>
          <a href="sign up.html" class="signup">Sign Up</a>
        </div>
      </nav>
    </header>
    <section class="hero-section">
      <div class="hero">
        <h2>Warmly Welcome !</h2>
        <p>
          Join us in the exciting website where you can change your whole life
          with colours and styles
        </p>
        <div class="buttons">
          <a href="sign in.html" class="join">Join Now</a>
          <a href="About.html" class="learn">Learn More</a>
        </div>
      </div>
      <div class="img">
        <img src="https://www.codingnepalweb.com/demos/create-responsive-website-html-css/hero-bg.png" alt="hero image" />
      </div>
    </section>
  </body>
</html>
