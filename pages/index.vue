<template>
    <div class ="bg">
        <div class="nav">
      <div class="nav__logo">iCube Systems</div>
      <a href="#" class="nav__hamburger">
        <span class="nav__hamburger__line"></span>
        <span class="nav__hamburger__line"></span>
        <span class="nav__hamburger__line"></span>
      </a>
      <div class="nav__menu">
        <ul>
          <li class="nav__menu__link"><a href="#index">Index</a></li>
   
          <li class="nav__menu__link"><a href="#about">About</a></li>
          <li class="nav__menu__link"><a href="#contact">Contact</a></li>
          
        </ul>
      </div>
        </div>
</div>
<div class= "news">
    <form class="login">
Start For Free
<h3>Welcome Back!</h3>
New User? <br></br>
        <div class= "start">
            <input type="text" placeholder="ID" />
        </div>
        <div>
            <input type="password" placeholder="Password" />
        </div>
    </form>

    <div class="slideshow">
    <el-carousel />
  </div>
 </div>
</template> 


<script setup>

 
</script>


<style scoped>


.news{
    display: flex;
    flex-direction:row;
    align-items: center;


}

.login {
    margin-top: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 87vh;
    width: 400px;
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
    border: 3px solid #ffffff;

    border-radius: 2ch;
    border: 2px solid #00000028;

  background: #ffffff;
  transition: background-color 2s ease-out 100ms
}

.login:hover {
  background-color: #bebebe;
}


.start{
    padding-top: 5px;
}
h3 {
    margin-top: 10px;
    margin-bottom: 10px;
}

input {
    margin-bottom: 10px;
    padding: 5px;
    border-radius: 5px;
    border: 1px solid #ccc;
}



/* NAVBAR */


.nav {
  height: 3.2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-image: linear-gradient(to right, rgb(0, 204, 255) , rgb(0, 4, 255));
  border-radius: 8px;

}

.nav__logo {
  font-size: 1.5rem;
  margin: auto 1rem;
}

.nav__menu ul {
  margin: 0;
  padding: 0;
  display: flex;
}

.nav__menu ul li {
  list-style: none;
}

.nav__menu ul li a {
  text-decoration: none;
  color: #fff;
  padding: 1rem;
  display: block;
}

.nav__menu li:hover {
  background-color: rgba(255, 255, 255, 0.5);
}

.nav__hamburger {
  width: 1.875rem;
  height: 1.313rem;
  display: none;
  flex-direction: column;
  justify-content: space-around;
  position: absolute;
  top: 1rem;
  right: 1rem;
}

.nav__hamburger__line {
  height: 0.188rem;
  width: 100%;
  background-color: #fff;
  border-radius: 0.625rem;
  transition: all ease-in-out 0.2s;
}






/* MEDIA QUERIES */

@media screen and (max-width: 550px) {
  .nav__hamburger {
    display: flex;
  }
  .nav__menu {
    position: absolute;
    display: flex;
    align-items: center;
    background-color: rgba(255, 255, 255, 0.2);
    top: -10rem;
    width: 100%;
    transition: all ease-in-out 0.4s;
  }
  .nav {
    flex-direction: column;
    align-items: flex-start;
  }
  .nav__menu ul {
    flex-direction: column;
    width: 100%;
    padding: 3rem 0 0.6rem;
  }
  .nav__menu ul li {
    text-align: center;
  }
  .nav__menu ul li a {
    padding: 0.5rem;
  }
  .nav__menu {
    z-index: -1;
  }
  .nav__menu.active {
    top: 0;
  }
  .nav__hamburger.active :nth-child(1) {
    transform: rotate(45deg) translate(0.45rem, 0.1875rem);
  }

  .nav__hamburger.active :nth-child(2) {
    opacity: 0;
  }

  .nav__hamburger.active :nth-child(3) {
    transform: rotate(-45deg) translate(0.45rem, -0.1875rem);
  }}

</style>

