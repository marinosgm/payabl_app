<template>
  <footer class="footer">
    <img src="@/assets/plogo.svg" alt="Your Company Logo" class="footer-logo">
    <div class="footer-columns">
      <!-- Dynamically create each column using v-for -->
      <div class="footer-column" v-for="(column, index) in footerColumns" :key="index">
        <p>{{ column.title }}</p>
        <p v-for="link in column.links" :key="link">{{ link }}</p>
      </div>
    </div>
    <img src="@/assets/social/linkedin.svg" alt="LinkedIn" class="social-icon" style="left: 2100px;">
    <img src="@/assets/social/facebook.svg" alt="Facebook" class="social-icon" style="left: 2180px;">
    <img src="@/assets/social/instagram.svg" alt="Instagram" class="social-icon" style="left: 2260px;">
    <img src="@/assets/social/twitter.svg" alt="Twitter" class="social-icon" style="left: 2340px;">
    <button class="newsletter-button">Join our newsletter</button>
    <p class="copyright-text">
      Copyright © payabl. 2023, all Rights Reserved.
    </p>
  </footer>
</template>
  
  <script>
 export default {
  data() {
    return {
      footerColumns: [
        { title: 'Products', links: ['Products', 'Capabilities', 'Integration', 'About', 'Capabilities', 'Integration', 'About'] },
        { title: 'Services', links: ['Products', 'Capabilities', 'Integration', 'About', 'Capabilities', 'Integration', 'About'] },
        { title: 'Resources', links: ['Products', 'Capabilities', 'Integration', 'About'] },
        { title: 'Company', links: ['Products', 'Capabilities', 'Integration', 'About'] }
      ]
    }
  }
};
  </script>
  
  <style scoped>
  /* Component-specific styles go here */
  .footer {
    margin-top: 300px;
    width: 100%;
    height: 661px;
    background-color: #E5EAE9;
    position: absolute;
    top: 6478px;
  }

  .footer-logo {
  position: absolute;
  width: 260px;
  height: 60px;
  top: 93px; /* Adjusted for relative positioning within the footer */
  left: 120px;
}

.footer-columns {
  display: grid;
  grid-template-columns: repeat(4, 91px);
  gap: 200px;
  position: absolute;
  top: 93px;
  left: 744px;
  width: calc(100% - 1044px);
  font-family: 'GinkaBold', sans-serif;
}

.footer-column {
  display: flex;
  flex-direction: column;
  justify-content: start;
  gap: 10px;
  max-height: 200px;
}

.footer-column p {
  margin: 5px 0;
}

.social-icon {
  position: absolute;
  width: 36.26px;
  height: 35.98px;
  top: 104px; /* 6582px - 6478px */
  
}

.newsletter-button {
  position: absolute;
  width: 260px;
  height: 43px;
  top: 176px; /* 6654px - 6478px */
  left: 2115px;
  padding: 12px;
  border-radius: 12px;
  border: 2px solid #022128;
  color: #022128;
  background-color: transparent; /* Adjust if you have a specific background color */
  font-size: 16px;
  text-align: center;
  font-family: 'GinkaBold', sans-serif;
}

.copyright-text {
  position: absolute;
  width: 297px;
  height: 19px;
  top: 470px; /* 6917px - 6478px */
  left: 746px;
  font-family: 'Karla', sans-serif;
  font-size: 12px;
  font-weight: 500;
  line-height: 18.03px;
  text-align: left;
  color: #022128;
}

@media (max-width: 768px) {


  .footer-logo {
    left: 50%; /* Center logo horizontally */
    transform: translateX(-50%); /* Align center */
  }

  .footer-columns {
    grid-template-columns: repeat(4, 1fr); /* 2 columns for easier navigation */
    gap: 50px; /* Reduced gap for better space utilization */
    left: 50px;
    top: 300px;
    }

  .social-icon {
    position: static; /* Static position for better flow */
    margin: 30px  ; /* Centering and adding margin */
    width: 32px; /* Adjust icon size for better visibility */
    height: 32px;
    margin-top: 610px;
    margin-left: 50px;
  }

  .newsletter-button {
    left: 50%; /* Center button horizontally */
    transform: translateX(-50%); /* Align center */
    top: 250px; /* Adjust top to not overlap other elements */
  }
}
@media (max-width: 480px) {
  .footer-logo {
    width: 150px; /* Adjust logo size to fit smaller screens */
  }

  .footer-columns {
    grid-template-columns: 1fr; /* Single column layout for clarity */
    gap: 50px; /* Reduced gap suitable for narrow screens */
    padding: 20px; /* Add padding to prevent elements from touching the screen edges */
  }

  .footer-column p {
    margin: 3px 0; /* Reduce margin to minimize space usage */
  }

  .social-icon {
    width: 28px; /* Slightly smaller icons */
    height: 28px;
    margin: 5px auto; /* Ensure consistent spacing around icons */
  }

  .newsletter-button {
    width: 180px; /* Smaller button width to fit mobile screens */
    top: 300px; /* Adjust placement to clear other footer elements */
  }
}
  </style>
  