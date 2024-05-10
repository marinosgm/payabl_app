<template>
    <div class="Testimonials">
      <!-- Testimonials content goes here -->
  
      <!-- First div box -->
      <div class="first-box">
        <button class="button" :style="{ backgroundColor: 'rgba(124, 221, 174, 0.2)', color: '#7CDDAE', opacity: '100%' }">Testimonials</button>
      <h2 class="heading">Real stories from real customers.</h2>
      <p class="paragraph">See what our partners are saying about our services.</p>
      </div>
      <!-- Second div box -->
      <div class="second-box">
        <div class="scroller">
    <div class="scroller-box" v-for="index in 6" :key="index">
        <!-- Existing content inside scroller-box -->

        <!-- New box with text -->
        <div v-if="index === 1" class="additional-box" style="font-size: 18px; font-weight: 400;">
            {{ getTextForIndex(1) }}

            <div class="new-div"></div>

            <div class="text">Name Surname</div>


        </div>
        
        <div v-if="index === 2" class="additional-box" style="font-size: 18px;font-weight: 400;">
            {{ getTextForIndex(2) }}
            <div class="new-div"></div>
            <div class="text">Name Surname</div>


        </div>
          
        <div v-if="index === 3" class="additional-box"  style="font-size: 18px;font-weight: 400;">
            {{ getTextForIndex(3) }}
            <div class="new-div"></div>
            <div class="text">Name Surname</div>


        </div>

        <div v-if="index === 4" class="additional-box" style="font-size: 18px;font-weight: 400;">
            {{ getTextForIndex(4) }}
            <div class="new-div"></div>
            <div class="text">Name Surname</div>


        </div>
        
        <div v-if="index === 5" class="additional-box"style="font-size: 18px;font-weight: 400;">
            {{ getTextForIndex(5) }}
            <div class="new-div"></div>
            <div class="text">Name Surname</div>


        </div>
          
        <div v-if="index === 6" class="additional-box"style="font-size: 18px;font-weight: 400;">
            {{ getTextForIndex(6) }}
            <div class="new-div"></div>
            <div class="text">Name Surname</div>


        </div>
    </div>
</div>


      </div>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
        getTextForIndex(index) {
            // Define an array of different texts
            const texts = [
                " “payabl. has proven its commitment to long-term merchant relationships. Throughout the many years of our collaboration, the payabl. team has maintained the same unrivaled standards in terms of customer service, responsiveness, system reliability, and risk management support, which are essential for our business.” ",
                " “payabl. has proven its commitment to long-term merchant relationships. Throughout the many years of our collaboration, the payabl. team has maintained the same unrivaled standards in terms of customer service, responsiveness, system reliability, and risk management support, which are essential for our business.” ",
                " “payabl. has proven its commitment to long-term merchant relationships. Throughout the many years of our collaboration, the payabl. team has maintained the same unrivaled standards in terms of customer service, responsiveness, system reliability, and risk management support, which are essential for our business.” ",
                " “payabl. has proven its commitment to long-term merchant relationships. Throughout the many years of our collaboration, the payabl. team has maintained the same unrivaled standards in terms of customer service, responsiveness, system reliability, and risk management support, which are essential for our business.” ",
                " “payabl. has proven its commitment to long-term merchant relationships. Throughout the many years of our collaboration, the payabl. team has maintained the same unrivaled standards in terms of customer service, responsiveness, system reliability, and risk management support, which are essential for our business.” ",
                " “payabl. has proven its commitment to long-term merchant relationships. Throughout the many years of our collaboration, the payabl. team has maintained the same unrivaled standards in terms of customer service, responsiveness, system reliability, and risk management support, which are essential for our business.” "
            ];

            // Return text based on the index
            return texts[index - 1]; // Adjust index to match array indexing
        }
    }
}
  </script>
  
  <style scoped>
    .Testimonials {

  justify-content: center;
  align-items: center;
      
    }

    .text {
  position: relative;
  width: 163px;
  height: 33px;
  top: 30px;
  left: 75px;
  font-size: 22px;
  font-family: 'GinkaBold', sans-serif; /* Setting Ginka as the font family */
  font-weight: 700;
  line-height: 33px;
  text-align: left;
}


    .new-div {
  position: relative;
  width: 53px;
  height: 53px;
  top: 73px;
  left: 0px;
  background: #D9D9D9;
  border-radius: 53px;
}
 
  /* First div box styles */
  .first-box {
  width: 902px;
  height: 264px;
  position: absolute;
  top: 4976px; /* Keep the top position as before */
  left: 50%; /* Position from left */
  transform: translateX(-50%); /* Center horizontally */
  text-align: center;
  display: flex; /* Use flexbox */
  flex-direction: column; /* Arrange children vertically */
  justify-content: center; /* Center vertically */
  align-items: center; /* Center horizontally */
  font-family: 'GinkaBold', sans-serif; /* Setting Ginka as the font family */
  margin-top: 100px;

}


  .button {

    top: -20px;
  width: 144px;
  height: 43px;
  gap: 10px;
  border: none;
  border-radius: 66px;
  font-family: 'Gink', sans-serif;
  font-size: 16px;
  font-weight: 700;
position: absolute;
  text-align: center;
  
}

.heading, .paragraph {
  width: 902px;
  height: 60px;
  font-family: 'Ginka', sans-serif;
  font-weight: 400;
  line-height: 54px;
  text-align: center;
  color: #FFFFFF;
}

.heading {
  position: absolute;
  font-size: 50px;
  font-family: 'GinkaRegular', sans-serif; /* Setting Ginka as the font family */
  top: 15px;

}

.paragraph {
  position: absolute;

  opacity: 50%;
  font-size: 18px;
  line-height: 27px;
  font-family: 'GinkaLight', sans-serif; /* Setting Ginka as the font family */
  top: 135px;

}
  
  /* Second div box styles */
  .second-box {
    position: absolute;
    width: 100%;
    height: 406px;
    top: 5334px;
    left: 50%;
    transform: translateX(-50%); /* Center horizontally */
    padding: 21px 0px 21px 36px;
    text-align: center;
  justify-content: center; /* Center vertically */
  align-items: center; /* Center horizontally */
  overflow: hidden; /* Hide content outside the box */

  }

  .scroller {
  width: 3996px;
  height: 364px;
  display: flex;
  gap: 24px;
  animation: scrollRight 40s infinite linear forwards; /* Animation for scrolling */

}

@keyframes scrollRight {
  0% {
    transform: translateX(50%);
  }
  25% {
    transform: translateX(0%);
  }
  50% {
    transform: translateX(-50%);
  }
  75% {
    transform: translateX(-75%);
  }
  100% {
    transform: translateX(50%);
  }
  
}

.scroller-box {
  width: 646px;
  height: 364px;
  gap: 0px;
  border-radius: 25px;
  background-color: #082C34;
}

.additional-box {
    position: relative;
    width: 518px;
    height: 172px;
    top: 50px;
    left: 41px;
    gap: 12px;
    color: white;
    text-align: left; /* Adjust text alignment as needed */
    padding: 0 8px; /* Add padding as needed */
    font-family: 'GinkaLight', sans-serif; /* Setting Ginka as the font family */

}




  </style>
  