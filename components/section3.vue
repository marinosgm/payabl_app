<template>
  <div class="section3">
    <div class="left-section">
      <button class="top-button">One Integration, Endless Solutions</button>
      <div class="box">
        <h2 :style="{ opacity: isButton2Clicked || isButton1Clicked ? 1 : 1,transition: 'opacity 0.5s ease-in-out'}">{{ title }}</h2>
        <p :style="{ opacity: isButton2Clicked ? 0.5 : 0.5 }">
          {{ paragraph }}
        </p>
      </div>
      <div class="buttons">
        <button class="button button1"@click="clickButton1":class="{ active: isButton1Active }"></button>
        <button class="button button2"@click="clickButton2":class="{ active: isButton2Active }"></button>
        <button class="button button3"@click="clickButton3"></button>
        <button class="button button4"@click="clickButton4"></button>
        <button class="button button5"@click="clickButton5"></button>
      </div>
    </div>
    <div class="right-section">
      <div class="main-box">
        <div class="box1">
          <img class="logo" src="@/assets/section3/logo2.svg" alt="Logo">
            <div class="text-box1">
          <h2 class="title">Choose Payment Method</h2>
          <p class="text">Please select the payment option that you prefer </p>
              </div>
        </div>
        <div class="box2"
             :class="{ 'hovered': isHovered }">
          <img class="pay" src="@/assets/section3/pay.svg" alt="Logo">
        </div>
        <button class="pay-button">Pay 45.50 EUR</button>
      </div>
    </div>
  </div>
</template>

<script setup >


import { ref, onMounted } from 'vue';



const isButton1Clicked = ref(false);
const isButton2Clicked = ref(false);
const isButton1Active = ref(true);
const isButton2Active = ref(false);
const title = ref("Payment products to meet every need.");
const paragraph = ref("Game-changing financial solutions for businesses with their eyes on global domination. Explore the endless payments possibilities with payabl. and level-up your business today.");

const isHovered = ref(false);


function clickButton1() {
  isButton1Clicked.value = true;
  isButton2Active.value = false;
  isButton1Active.value = true;
  if (isButton1Clicked.value) {
      title.value = "Payment products to meet every need.";
      paragraph.value = "Game-changing financial solutions for businesses with their eyes on global domination. Explore the endless payments possibilities with payabl. and level-up your business today.";
    } 
  // Handle Button 1 click event if needed
}

function clickButton2() {
  isButton2Clicked.value = true;
  isButton1Active.value = false;
  isButton2Active.value = true;
  if (isButton2Clicked.value) {
  title.value = "Security built in its core";
  paragraph.value = "Game-changing financial solutions for businesses with their eyes on global domination. Explore the endless payments possibilities with payabl. and level-up your business today.";
  }
}

function clickButton3() {
  // Handle Button 3 click event if needed
}

function clickButton4() {
  // Handle Button 4 click event if needed
}

function clickButton5() {
  // Handle Button 5 click event if needed
}

function handleMouseEnter() {
  isHovered.value = true;
}

// Function to handle mouse leave event
function handleMouseLeave() {
  isHovered.value = false;
}

onMounted(() => {
  let interval = setInterval(() => {
    isHovered.value = !isHovered.value;
    if (isHovered.value) {
      setTimeout(() => {
        isHovered.value = false;
      }, 5000); // remains large for 5 seconds, total 10 seconds cycle
    }
  }, 5000); // 5 seconds small, 5 seconds transition to large, 5 seconds large

  // Cleanup on component unmount
  onBeforeUnmount(() => {
    clearInterval(interval);
  });
});

</script>


<style scoped>
.section3 {
  position: relative;
  width: 871px;
  height: 811px;
  margin-top: 350px;
}
.left-section {
  position: absolute;
  width: 877px;
  height: 100%;
  left: 30%;
  justify-content: center;
  padding: 0px 48px;
  text-align: left;
}

.top-button {
  width: 309px;
  height: 43px;
  padding: 12px 24 12px 24px;
  gap: 10px;
  border-radius: 66px;
  background: #08ee7f33;
  color: #7CDDAE;
  left: 261px;
  font-weight: 700;
  font-family: 'Ginka', sans-serif;
  align-self: center;
  border: none;



}
h2 {
  width: 466px;
  height: 120px;
  font-size: 50px;
  font-weight: 400;
  line-height: 60px;
  text-align: left;
  color: white;
  font-family: 'Ginka', sans-serif;
  

}

p {
  width: 540px;
  height: 105px;
  font-family: 'Ginka', sans-serif;
  font-size: 18px;
  font-weight: 400;
  line-height: 27px;
  text-align: left;
  color: white;
  opacity: .5;
}

h2, p {
  transition: ease-in-out 1s;
}

.buttons {
  position: absolute;
  gap: 14px;
  display: flex;
  


}

.button {
  width: 186px;
  height: 16px;
  gap: 14px;
  border-radius: 33px;
  background: #D9D9D9;
  border: none;
  cursor: pointer;
  
}

.button1 {
  width: 66px;
  height: 16px;
  gap: 20px;
  border-radius: 33px;
  background: #7CDDAE;
}

.button2,.button3,.button4,.button5 {
  width: 16px;
  height: 16px;
  border-radius: 33px;
  opacity:30%;
  background-color: #D9D9D9;
  gap: 20px;

}

.button1.active,.button2.active,.button3.active,.button4.active,.button5.active {
  width: 66px;
  height: 16px;
  gap: 20px;
  border-radius: 33px;
  background: #7CDDAE;
  opacity: 100%;
  animation: fade-in


}

.button1,.button2,.button3,.button4,.button5.inactive {
  width: 16px;
  height: 16px;
  border-radius: 33px;
  opacity: 30%;
  background-color: #D9D9D9;
  gap: 20px;
  transition: ease-in-out .5s;
}

.right-section {
  width: 700px;
  height: 700px;
  position: absolute;
  right: 0;
  top: 0;
  left: 1600px;
}


.main-box {
  position: absolute;
  width: 428px;
  height: 467px;
  background-color: white;
  border-radius: 51.65px;
  padding: 51.65px;
  gap: 80.35px;
}
.box1 {
  width: 344px;
  height: 167px;
  position: absolute;
  background-color: rgb(255, 255, 255);
  color: black;
}

.box1.logo {
  width: 150px;
  height: 34px;
  transform: rotate(0deg);
}



.box2 { width: 453px;
  height: 88px;
  background-color: white;
  border-radius: 16px;
  position: relative;
  top: 65%;
  left: 50%;
  transform: translate(-50%, -50%); 
  justify-content: center;
  align-items: center;
  padding: 10px;
  transition: width 0.6s, height 0.5s, border-radius 0.5s, border 0.1s;
  
}
.hovered {
  width:700.53px; /* Desired width */
  height: 107px; /* Desired height */
  border: 1.3px solid #7CDDAE; /* Desired border */
}

.pay {
  display: block;
  width: 100%; /* Make the image fill the box */
  height: 100%; /* Make the image fill the box */
}
.box2 .pay {
  position: relative;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  
}

.pay-button {
  width: 424.7px;
  height: 66px;
  border-radius: 10.04px;
  position: absolute;
  top: 85%;
  left: 50%;
  transform: translate(-50%, -50%);
  border: none;
  cursor: pointer;
  font-size: 25.96px;
  font-weight: 700;
  font-family: 'Ginka', sans-serif;  
  justify-content: center;
  align-items: center;
  background-color: #7CDDAE;
  
}

.logo{

  width: 150.65px;
height: 34.43px;
top: 51.65px;
left: 52.15px;

 
}



.title{
  height: 40px;
  width: 344px;
  font-size: 26px;
  font-weight: 700;
  text-align: left;
  color: rgb(0, 0, 0);
  font-family: 'Ginka', sans-serif;
  margin-top: 40px;


}

.text{
  height: 42px;
  width: 319px;
  font-family: 'Ginka', sans-serif;
  font-size: 18px;
  font-weight: 700;
  text-align: left;
  color: rgb(0, 0, 0);
  opacity: .5;
    
}

@media only screen and (max-width: 768px) {
  .section3 {
    width: 100%; /* Adjust the section width to full viewport width */
    height: auto; /* Make height auto to accommodate content */
    margin-top: 50px; /* Reduce top margin */
  }

  .left-section, .right-section {
    position: relative;
    width: 100%; /* Make both sections full width */
    left: 0; /* Reset left positioning */
    padding: 0 20px; /* Add padding for internal spacing */
  }

  .top-button {
    width: auto; /* Adjust button width to fit content */
    margin: 0 auto; /* Center the button */
  }

  .buttons {
    justify-content: space-around; /* Adjust button spacing */
  }

  .button1, .button2, .button3, .button4, .button5 {
    width: 50px; /* Adjust the size of the buttons */
    height: 14px; /* Adjust the height of the buttons */
  }

  .main-box {
    width: 90%; /* Adjust the width of the main box */
    margin: 20px auto 0; /* Center the main box with margin */
    padding: 20px; /* Adjust padding */
    gap: 20px; /* Adjust gaps between elements */
  }

  .box1, .box2 {
    width: 100%; /* Adjust widths of these boxes to be full */
  }

  .pay-button {
    width: 100%; /* Make the pay button full width */
    margin-top: 20px; /* Add top margin */
  }

  .text, .title {
    font-size: 16px; /* Adjust the font size for readability */
  }
}


</style>