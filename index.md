<header>
  <!-- Menu Chexkbox -->
  <input type="checkbox" id="menu-show">
  <!-- Logo -->
  <a href="#" class="logo">
    <img src="https://i.ibb.co/YD6DNKk/logo.png" alt="">
  </a>
  <!-- Menu Links -->
  <ul class="menu">
    <li><a href="#">Home</a></li>
    <li><a href="#">Burgers</a></li>
    <li><a href="#">Fries</a></li>
    <li><a href="#">Drinks</a></li>
  </ul>
  <!-- Menu Icons -->
  <label for="menu-show"><i class="fas fa-bars"></i></label>
  <label for="menu-show"><i class="fas fa-times"></i></label>
</header>
<!-- Image Slide Radio -->
<input type="radio" id="burger" name="rd" checked>
<input type="radio" id="fries" name="rd">
<input type="radio" id="coke" name="rd">
<!-- Container -->
<div class="container">
  <!-- Text -->
  <div class="text-box">
    <h2>Enjoyable lunch <br>It's <span>KFC</span></h2>
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Doloremque fuga nobis nihil libero eveniet aperiam ex repudiandae praesentium quaerat cum excepturi, quas fugit. Et odio repudiandae ea quibusdam vero consectetur, nemo, ullam perspiciatis laudantium obcaecati.</p>
    <a href="#">Order Now</a>
  </div>
  <!-- Images -->
  <div class="bg-img">
    <img src="https://i.ibb.co/b7DDN0T/burger.png" alt="">
    <img src="https://i.ibb.co/B4TZNx2/fries.png" alt="">
    <img src="https://i.ibb.co/M73ZR04/coke.png" alt="">
  </div>
</div>
<!-- Image Slide -->
<ul class="thumb">
  <li><label for="burger"><img src="https://i.ibb.co/b7DDN0T/burger.png" alt=""></label></li>
  <li><label for="fries"><img src="https://i.ibb.co/B4TZNx2/fries.png" alt=""></label></li>
  <li><label for="coke"><img src="https://i.ibb.co/M73ZR04/coke.png" alt=""></label></li>
</ul>
<!-- Shapes -->
<div class="shape red"></div>
<div class="shape yellow"></div>
<div class="shape orange"></div>
<!-- Footer -->
<footer>
  <!-- Social Icons -->
  <div class="social">
    <a href="#"><i class="fab fa-facebook-square"></i></a>
    <a href="#"><i class="fab fa-twitter-square"></i></a>
    <a href=""><i class="fab fa-instagram-square"></i></a>
    <a href=""><i class="fab fa-linkedin"></i></a>
  </div>
  <!-- Credit Text -->
  <div class="credit">
    <p>Copyright &copy; 2021 - KFC</p>
    <p>Designed & Developed by WAHS</p>
  </div>
</footer>
<style>

@import url("https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;1,100;1,300;1,400&display=swap");

/* -----Reset----- */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Roboto", sans-serif;
}

/* -----Common----- */
body {
  background-color: #fff;
  width: 100%;
  min-height: 100vh;
}

a {
  text-decoration: none;
  color: #000;
  transition: all 0.3s ease-in;
}

li {
  list-style: none;
  cursor: pointer;
  transition: all 0.3s ease-in;
}

li:hover {
  transform: scale(1.1);
}

label {
  cursor: pointer;
}

input[type="radio"],
input[type="checkbox"] {
  display: none;
}

/* -----Header----- */
header {
  width: 100%;
  padding: 20px 200px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  overflow-x: hidden;
}

/* Logo */
header .logo {
  position: relative;
  z-index: 101;
  max-width: 80px;
  text-align: center;
}

header .logo img {
  width: 100%;
}

/* Menu Links */
header .menu {
  max-width: 300px;
  position: relative;
  z-index: 101;
  display: flex;
  justify-content: center;
  align-items: center;
}

header .menu li {
  margin: 0 15px;
  padding: 10px 20px;
}

/* Menu Icons */
header label {
  position: absolute;
  z-index: 101;
  top: 40px;
  right: 50px;
  display: none;
}

header label i {
  font-size: 1.5rem;
  color: #000;
}

/* -----Container----- */
.container {
  position: relative;
  z-index: 100;
  min-height: 75vh;
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  padding: 0 20px;
  margin-bottom: 100px;
  overflow: hidden;
}

/* Text */
.container .text-box {
  width: 600px;
  padding: 20px;
  text-align: left;
}

.container .text-box h2 {
  font-size: 4rem;
}

.container .text-box h2 span {
  padding: 0 15px;
  background-color: #000;
  color: #fff;
}

.container .text-box p {
  font-size: 1rem;
  margin: 10px 0;
}

.container .text-box a {
  display: inline-block;
  padding: 20px 50px;
  border: 3px #000 solid;
  color: #000;
}

.container .text-box a:hover {
  background-color: #000;
  color: #fff;
}

/* Images */
.container .bg-img {
  max-width: 550px;
  width: 100%;
  overflow: hidden;
}

.container .bg-img img {
  width: 100%;
  transition: all 0.5s ease-in;
}

.container .bg-img img:nth-child(3) {
  width: 90%;
}

/* Shapes */
.shape {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 100%;
  clip-path: circle(60% at right);
  transition: all 0.5s ease-in;
}

.red {
  background-color: #c0392b;
}

.yellow {
  background-color: #f39c12;
}

.orange {
  background-color: #d35400;
}

/* -----Fixed Image Slide Menu----- */
.thumb {
  position: fixed;
  top: 50%;
  transform: translateY(-50%);
  right: 5px;
  padding: 10px;
  z-index: 101;
}

.thumb li {
  margin: 10px 0;
  transition: all 0.3s ease-in;
}

.thumb img {
  max-width: 50px;
}

/* Footer */
footer {
  width: 100%;
  position: fixed;
  z-index: 101;
  bottom: 0;
  left: 0;
  padding: 20px;
  display: flex;
  justify-content: center;
  align-items: flex-end;
  flex-direction: column;
}

/* Social Icons */
footer .social {
  margin-bottom: 10px;
}

footer .social a {
  margin-left: 20px;
}

footer .social i {
  color: #000;
  font-size: 1.6rem;
  transition: all 0.3s ease-in;
}

footer .social i:hover {
  transform: scale(1.1);
}

/* Credit Text */
footer .credit {
  text-align: right;
  color: #000;
  font-size: 0.9rem;
}

/* -----Image Slide----- */
/* First Image */
#burger:checked ~ .container .bg-img img:nth-child(1) {
  visibility: visible;
  opacity: 1;
}

#burger:checked ~ .container .bg-img img:nth-child(2),
#burger:checked ~ .container .bg-img img:nth-child(3),
#burger:checked ~ .orange,
#burger:checked ~ .yellow {
  max-height: 0;
  visibility: hidden;
  opacity: 0;
}

/* Second Image */
#fries:checked ~ .container .bg-img img:nth-child(2) {
  visibility: visible;
  opacity: 1;
}

#fries:checked ~ .container .bg-img img:nth-child(1),
#fries:checked ~ .container .bg-img img:nth-child(3),
#fries:checked ~ .red,
#fries:checked ~ .orange {
  max-height: 0;
  visibility: hidden;
  opacity: 0;
}

/* Third Image */
#coke:checked ~ .container .bg-img img:nth-child(3) {
  visibility: visible;
  opacity: 1;
}

#coke:checked ~ .container .bg-img img:nth-child(1),
#coke:checked ~ .container .bg-img img:nth-child(2),
#coke:checked ~ .red,
#coke:checked ~ .yellow {
  max-height: 0;
  visibility: hidden;
  opacity: 0;
}

/* -----Responsive----- */
@media (max-width: 950px) {
  /* Header */
  header {
    flex-direction: column;
    padding: 20px 50px;
  }

  header .logo {
    margin-bottom: 10px;
  }

  /* Container */
  .container {
    flex-direction: column;
  }

  .container .text-box {
    width: 100%;
    max-width: 550px;
    text-align: center;
  }

  .container .bg-img {
    max-width: 450px;
    width: 100%;
  }

  .container .bg-img img:nth-child(3) {
    width: 100%;
  }

  /* Footer */
  footer {
    position: relative;
  }
}

@media (max-width: 470px) {
  /* Header */
  header .menu {
    position: absolute;
    width: 100%;
    max-width: inherit;
    flex-direction: column;
    background-color: #fff;
    padding: 10px 0;
    top: 120px;
    left: -100%;
    transition: all 0.3s ease-in;
  }

  header .menu li {
    margin: 15px 0;
  }

  header label:nth-child(4) {
    display: block;
  }

  /* Container */
  .container .text-box h2 {
    font-size: 3rem;
  }

  /* Fixed Image Slide Menu */
  .thumb img {
    max-width: 30px;
  }

  /* Responsive Menu */
  #menu-show:checked ~ .menu {
    left: 0;
  }

  #menu-show:checked ~ label:nth-child(4) {
    display: none;
  }

  #menu-show:checked ~ label:nth-child(5) {
    display: block;
  }
}

	</style>
