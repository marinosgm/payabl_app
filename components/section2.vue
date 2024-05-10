<template>
    <div class="section2">
      <div class="top-section">
        <h2>All about payable. and what we do</h2>
        <p>
          Our wide range of payments products includes card acquiring, banking
          services, local payment methods, and POS terminals. We supercharge your
          business growth with our easy-to-install payment tech, smart fraud
          prevention, and dedicated customer support. Welcome to payabl. where we
          take care of the payments, so you can take care of business.
        </p>
      </div>
      <div class="bottom-section">
        <img src="@/assets/section2/img2.svg" alt="Logo">
      </div>
    </div>
  </template>
  
  <script >
  export default {
    name: 'Section2',
  };

  </script>

  <style scoped>
  .section2 {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px;
    margin-top: -60px; /* Move the component up by 20px */


  }
  
  .top-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 1124px;
    height: 153px;
    margin-bottom: 150px;
    margin-top: 100px;
  }
  
  h2 {
    font-size: 40px;
    margin-bottom: 10px;
    width: 924px;
    height: 48px;
    text-align: center;
    color: white;
    font-weight: 400;
    font-family: 'GinkaRegular', sans-serif;
  }
  
  p {
    font-size: 16px;
    line-height: 1.5;
    width: 1124px;
    height: 83px;
    text-align: center;
    color: white;
    opacity: .5;
    font-weight: 400;
  }
  
  .bottom-section {
    
width: 100%;
height: Hug (220.2px)px;
top: 1477px;
left: -48px;
gap: 135px;
opacity: .5;


  }
  
  img {
    width: 100%;
    height: auto;
  }

  @media (max-width: 768px) {
  .top-section {
    width: 90%; /* Adjust width to be responsive */
    margin-bottom: 50px; /* Less space on smaller screens */
    margin-top: 100px;
  }

  img {
    
    margin-top: 100px;
  }

  h2 {
    font-size: 24px; /* Smaller font size for smaller screens */
    width: 90%; /* Responsive width */
  }

  p {
    font-size: 14px; /* Smaller font size */
    width: 90%; /* Responsive width */
    height: auto; /* Allow height to adjust based on content */
  }

  .bottom-section {
    top: auto;
    left: 0;
    gap: 100px; /* Reduced gap */
  }
}
</style>