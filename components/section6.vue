<template>
    <div class="section6">
      <div class="main-box" @mouseover="hoverEffect" @mouseleave="resetEffect">
        <!-- Your Section6 content goes here -->
        <div class="content-box">
        <p class="business-text">See how we can help grow your business.</p>
        <button class="cta-button">Contact Us</button>
      </div>
      </div>
    </div>
  </template>
  
  <script>
 export default {

};
  </script>
  
  <style scoped>
  /* Component-specific styles go here */
  .section6 {
  display: flex;
  align-items: center;
  justify-content: center;
}

    
  
  
  .main-box {
    width: 1396px;
    height: 368px;
    position: relative;
    aspect-ratio: 1396 / 368; /* Maintain aspect ratio based on original dimensions */

    top: 2000px;
    border-radius: 25px;
    background-image: url("~/assets/section6/group (6).png"); /* Set background image */
    background-repeat:no-repeat;
    background-position: 200px center;
    background-color: white;
          margin-top: -100px;
          transition: all 1s;


  }

  .main-box:hover {
    background-position: 0px center;
}

.content-box {
    width: 902px;
    height: 189px;
    position: absolute;
    top: 80px;
    left: 75px;
    display: flex;
    flex-direction: column;
    gap: 36px;
  }

  /* Styling for the text inside content box */
  .business-text {
    width: 902px;
    height: 110px;
    font-family: 'GinkaBold', sans-serif; /* Setting Ginka as the font family */
    font-size: 50px;
    font-weight: 700;
    line-height: 55px;
    text-align: left;
    color: #022128;
    position: absolute;
    top: -40px;
  }

  /* Button inside content box */
  .cta-button {
    width: 135px;
    height: 43px;
    padding: 12px 24px;
    border-radius: 12px;
    background-color: #7CDDAE;
    font-size: 16px; /* Specify font-size if needed */
    color: #022128; /* Text color */
    border: none; /* Remove default border */
    cursor: pointer; /* Pointer cursor on hover */
    position: absolute;
    top: 170px;
    font-family: 'GinkaBold', sans-serif; /* Setting Ginka as the font family */
    font-size: 16px;
    line-height: 19.2px;
    text-align: center;
    color: #022128; /* Text color */
    border: none; /* Remove default border */
    cursor: pointer; /* Pointer cursor on hover */
    
  }

/* Media queries for tablet devices */
@media (max-width: 1024px) {
    .main-box {
      width: 90%; /* Adjust width for smaller devices */
      height: auto; /* Height becomes flexible */
      top: 1000px; /* Less extreme positioning */
      margin-top: 0; /* Remove negative margin */
    }

    .content-box {
      width: 80%; /* Reduce width to fit new container size */
      top: 1150px; /* Adjust top position */
      left: 10%; /* Center content horizontally */
    }

    .business-text {
      font-size: 40px; /* Decrease font size */
      top: 0; /* Adjust position */
    }

    .cta-button {
      top: 150px; /* Adjust button position downwards */
    }
  }

  /* Media queries for mobile devices */
  @media (max-width: 768px) {
    .main-box {
      width: auto;
      top: 2800px; /* Less extreme positioning */
    }

    .content-box {
      top: 20px; /* Adjust top position */
      left: 5%; /* Center content more appropriately */
    }

    .business-text {
      font-size: 30px; /* Further decrease font size */
    }

    .cta-button {
      top: 120px; /* Adjust button position further */
      width: 100px; /* Adjust button width */
      padding: 10px 20px; /* Adjust padding */
    }
  }

  </style>
  