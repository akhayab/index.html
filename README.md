
<!-- Navigation Menu -->
<nav class="navbar">
  <div class="nav-logo">
    <img src="images/protest_logo.jpg" alt="Janawaz Logo" class="nav-logo-img">
    <span class="nav-title">ଜନଆଵାଜ</span>
  </div>
  <div class="menu-toggle" id="menu-toggle">&#9776;</div>
  <ul class="nav-links" id="nav-links">
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#protest">Protest</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>

<!-- Header Section -->
<header class="hero">
  <h1 class="site-title">ଜନଆଵାଜ</h1>
  <p class="tagline">ଆମ ଆଵାଜ ଆମ ଶକ୍ତି</p>

  <div class="buttons">
    <a href="#join" class="btn join-btn">&#128100; Join Now</a>
    <a href="#raise" class="btn raise-btn">&#128226; Raise Your Voice</a>
  </div>
</header>

<!-- CSS Section -->
<style>
/* Navbar Styles */
.navbar {
  background: #0052D4;
  padding: 10px 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: relative;
  box-shadow: 0 4px 8px rgba(0,0,0,0.3);
}

.nav-logo {
  display: flex;
  align-items: center;
}

.nav-logo-img {
  height: 40px;
  border-radius: 50%;
  margin-right: 10px;
}

.nav-title {
  color: white;
  font-size: 22px;
  font-weight: bold;
  font-family: 'Noto Sans Oriya', sans-serif;
}

.menu-toggle {
  display: none;
  font-size: 28px;
  color: white;
  cursor: pointer;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 20px;
}

.nav-links li a {
  color: white;
  text-decoration: none;
  font-size: 16px;
  font-weight: bold;
  transition: color 0.3s;
}

.nav-links li a:hover {
  color: #ffde59;
}

/* Header Section */
.hero {
  background: linear-gradient(90deg, #0052D4, #4364F7, #6FB1FC);
  padding: 30px 20px;
  text-align: center;
  animation: fadeIn 2s ease;
}

.site-title {
  color: white;
  font-family: 'Noto Sans Oriya', sans-serif;
  font-size: 34px;
  margin-top: 20px;
}

.tagline {
  color: #f0f0f0;
  font-family: 'Noto Sans Oriya', sans-serif;
  font-size: 20px;
  margin-top: 5px;
}

/* Buttons */
.buttons {
  margin-top: 25px;
}

.btn {
  padding: 12px 25px;
  border-radius: 30px;
  text-decoration: none;
  font-weight: bold;
  font-size: 18px;
  display: inline-flex;
  align-items: center;
  gap: 8px;
  transition: 0.4s;
  margin: 8px;
}

.join-btn {
  background: linear-gradient(to right, #ffffff, #d1d1d1);
  color: #0052D4;
}

.raise-btn {
  background: linear-gradient(to right, #ff4081, #ff6f91);
  color: #ffffff;
}

.btn:hover {
  transform: scale(1.05);
  box-shadow: 0 8px 16px rgba(0,0,0,0.3);
}

/* Responsive Design */
@media (max-width: 768px) {
  .nav-links {
    flex-direction: column;
    background: #0052D4;
    position: absolute;
    top: 60px;
    right: 20px;
    width: 200px;
    display: none;
    padding: 10px;
    border-radius: 8px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.5);
  }

  .nav-links.active {
    display: flex;
  }

  .menu-toggle {
    display: block;
  }
}

@media (max-width: 600px) {
  .hero {
    padding: 20px 10px;
  }

  .site-title {
    font-size: 26px;
  }

  .tagline {
    font-size: 16px;
  }

  .btn {
    font-size: 16px;
    padding: 10px 20px;
  }
}

/* Animations */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}
</style>

<!-- JavaScript Section -->
<script>
const toggleBtn = document.getElementById('menu-toggle');
const navLinks = document.getElementById('nav-links');

toggleBtn.addEventListener('click', () => {
  navLinks.classList.toggle('active');
});
</script>
