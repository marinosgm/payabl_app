<template>
    <nav>
        <div class="logo">
            <img src="@/assets/navbar/logo.svg" alt="Logo">
    </div>
    <ul>
      <li><nuxt-link to="/">Products</nuxt-link></li>
      <li><nuxt-link to="/about">Capabilities</nuxt-link></li>
      <li><nuxt-link to="/about">Integration</nuxt-link></li>
      <li><nuxt-link to="/about">About</nuxt-link></li>

    </ul>
    <div class="right-side">
      <button class="login-button">Login</button>
      <button class="contact-button">Contact Us</button>
    </div>
  </nav>
  </template>
  
  <script>
  import { onMounted } from 'vue';
  
  export default {
    setup() {
      onMounted(() => {
        const navbar = document.querySelector('nav');
        let navbarScrolled = false;
  
        window.addEventListener('scroll', () => {
          if (window.scrollY > 60) {
            if (!navbarScrolled) {
              navbar.classList.add('scrolled');
              navbarScrolled = true;
            }
          } else {
            if (navbarScrolled) {
              navbar.classList.remove('scrolled');
              navbarScrolled = false;
            }
          }
        });
      });
    },
  };
  </script>

  <style scoped>


nav {
    display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: --primary-color;
  color: #fff;
  padding-left:120px;
  padding-right:120px;   
  padding-top: 10px;
  padding-bottom: 10px;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 999;
  transition: top 0.3s ease-in-out;
  max-width: 100%;
  
}

nav.scrolled {
  background-color: #022128; /* Keep the background color when scrolled */
  top: 0;
}

.logo {
  margin-right: 10px;
}

.logo img {
  height: 30px;
}

ul {
  display: flex;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

li {
  margin: 0 100px;
  font-weight: 700;
  font-size: 16px;
  font-family: 'GinkaBold', sans-serif;
}

a {
  color: #fff;
  text-decoration: none;
}


.right-side {
  display: flex;
  align-items: center;
}

.login-button,
.contact-button {
  margin-left: 10px;
  padding: 0 24px;
  border: 2px solid #fff;
  border-radius: 12px;
  height: 43px;
  line-height: 39px;
  background-color: transparent;
  color: white;
  cursor: pointer;
  font-family: 'GinkaBold', sans-serif;
  font-size: 16px;
}

.contact-button {
  background-color: #7cddae;
  border: 2px solid #7cddae;
  border-radius: 12px;
  color: #022128;
  font-weight: 700;
  height: 43px;
  line-height: 39px;
  text-align: center;
}


@media (max-width: 768px) {
  li {
    margin: 0 5px;
    max-width: 100%;

  }
}


</style>