<template>
  <div>
    <Navbar />
    <Section1></Section1>
    <Section2></Section2>
    <Section3></Section3>
    <Section4></Section4>
    <Section5></Section5>
    <Testimonials></Testimonials> <!-- Add Testimonials component here -->
    <Section6></Section6> <!-- Add Section6 component here -->
    <Footer></Footer> <!-- Add Footer component here -->




  </div>

 
</template>

<script>
import Navbar from '~/components/Navbar.vue';
import Section1 from '~/components/section1.vue'; // Import the Section1 component
import Section2 from '~/components/section3.vue';
import Section3 from '~/components/section3.vue';
import Section4 from '~/components/section4.vue';
import Section5 from '~/components/section5.vue';
import Testimonials from '~/components/Testimonials.vue'; // Import the Testimonials component
import Section6 from '~/components/section6.vue'; // Import the Section6 component
import Footer from '~/components/Footer.vue'; // Import the Footer component




export default {
  components: {
    Navbar, 
    Section1,
    Section2,
    Section3, 
    Section4,
    Section5,
    Testimonials, // Register the Testimonials component
    Section6, // Register the Section6 component
    Footer, // Register the Footer component



  

  },
};
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Ginka&display=swap');


:root {
  --primary-color: #022128;
  --font-family: 'Ginka-Bold', sans-serif;
  --font-family2: 'Ginka', sans-serif;
}

body {
  margin: 0;
  padding: 0;
  background-color: var(--primary-color);
  font-family: 'Ginka', sans-serif;


}

  @font-face {
    font-family: 'GinkaBold';
    src: url('/assets/fonts/Ginka-Bold.otf') format('opentype');
    font-weight: 700;
    font-style: normal;
}

@font-face {
    font-family: 'GinkaLight';
    src: url('/assets/fonts/Ginka-Light.otf') format('opentype');
    font-weight: 400;
    font-style: normal;
}

@font-face {
    font-family: 'GinkaMedium';
    src: url('/assets/fonts/Ginka-Medium.otf') format('opentype');
    font-weight: 400;
    font-style: normal;
}

@font-face {
    font-family: 'GinkaBook';
    src: url('/assets/fonts/Ginka-Book.otf') format('opentype');
    font-weight: 400;
    font-style: normal;
}

@font-face {
    font-family: 'GinkaRegular';
    src: url('/assets/fonts/Ginka-Regular.otf') format('opentype');
    font-weight: 400;
    font-style: normal;
}

</style>
