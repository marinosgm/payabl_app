<template>
  <div class="section5">
    <div class="box1">
      <button class="button" :style="{ backgroundColor: 'rgba(124, 221, 174, 0.2)', color: '#7CDDAE', opacity: '100%' }">Testimonials</button>
      <h2 class="heading">Real stories from real customers.</h2>
      <p class="paragraph">See what our partners are saying about our services.</p>
    </div>
    <div class="box2" :style="{ width: '1192.18px', height: '715px', top: '220px', gap: '0px', position: 'absolute'}">
      <div class="main-box":style="{ borderColor: activeButtonColor }">
        <div class="order-summary-box":style="{ backgroundColor: activeButtonColor }">
          <div class="eur-20">
            <div class="text-20":style="{ color: activeButton === 3 ? 'rgb(2, 33, 40)' : 'white' }">20</div>
            <div class="text-eur":style="{ color: activeButton === 3 ? 'rgb(2, 33, 40)' : 'white' }">EUR</div>
          </div>
          <div class="order-summary" :style="{ width: '225.38px', height: '119.68px', top: '292.99px', left: '32.64px', position: 'absolute'}">
            <h2 class="order-summary-title":style="{ color: activeButton === 3 ? 'rgb(2, 33, 40)' : 'white' }">Order Summary</h2>
            <p class="order-summary-text":style="{ color: activeButton === 3 ? 'rgb(2, 33, 40)' : 'white' }">Here is what you have added to your shopping cart.</p>
            <img src="@/assets/section5/order.svg" alt="Order" class="order-image" :style="{ width: '94.11px', height: '70.58px', top: '342.1px', left: '32.64px', borderRadius: '5.29px' }" />
            <div class="rect1":style="{ backgroundColor: activeButton === 3 ? 'rgb(2, 33, 40)' : 'white' }"></div>
            <div class="rect2":style="{ backgroundColor: activeButton === 3 ? 'rgb(2, 33, 40)' : 'white' }"></div>
          </div>

          <div class="summary-footer" :style="{ width: '269.93px', height: '24.87px', top: '447.65px', left: '25.64px', gap: '0px', borderRadius: '40.03px', backgroundColor: 'transparent', position: 'absolute' }">
            <img src="@/assets/section5/language.svg" alt="Language" :style="{ width: '74.13px', height: '24.87px',  borderRadius: '40.03px',position: 'absolute',left: '0px' }" />
            <div class="divbox1" :style="{ width: '71.5px', height: '11.66px', left: '100.56px', position: 'absolute' }">
            
              <!-- Vector1.svg -->
            <img
      v-if="activeButton === 3"
      src="@/assets/section5/Vector1 copy.svg"
      alt="Vector1"
      class="Vector1"
      :style="{ width: '23.72px', height: '11.66px', top: '5.88px', left: '0px', position: 'absolute', fill: 'black' }"
    />
    <img
      v-else
      src="@/assets/section5/Vector1.svg"
      alt="Vector1"
      class="Vector1"
      :style="{ width: '23.72px', height: '11.66px', top: '5.88px', left: '0px', position: 'absolute', fill: 'white' }"
    />
            <!-- Vector (1).svg -->
            
            <img
      v-if="activeButton === 3"
      src="@/assets/section5/Vector (1) copy.svg"
      alt="Vector2"
      class="Vector2"
      :style="{ width: '32.91px', height: '9.62px', top: '5.88px', left: '38.59px', position: 'absolute', fill: 'black' }"
    />
    <img
      v-else
      src="@/assets/section5/Vector (1).svg"
      alt="Vector2"
      class="Vector2"
      :style="{ width: '32.91px', height: '9.62px', top: '5.88px', left: '38.59px', position: 'absolute', fill: 'white' }"
    />
    <img
      v-if="activeButton !== 3"
      src="@/assets/section5/logoo.svg"
      alt="Logo"
      class="logo"
      :style="{ width: '56.2px', height: '19.43px', top: '0px', left: '95px', padding: '0px', position: 'absolute' }"
    />
    <img
      v-else
      src="@/assets/section5/logoo copy.svg"
      alt="Logo Copy"
      class="logo-copy"
      :style="{ width: '56.2px', height: '19.43px', top: '0px', left: '95px', padding: '0px', position: 'absolute' }"
    />

        </div>
            
          </div>

        </div>
        <div class="checkout" :style="{ width: '217px', height: '404.51px', top: '40.52px', left: '454.65px',position: 'absolute' }">
         
            <h2 class="quick-pay" :style="{ width: '61.07px', height: '11px', top: '50.52px', left: '457.76px',  fontSize: '9.33px', fontWeight: 700, lineHeight: '11.19px', textAlign: 'left', color: 'white',fontFamily: 'GinkBold, sans-serif' }">Quick Pay</h2>
          
              <img src="@/assets/section5/gapay.svg" alt="Gapay" class="gapay-image" :style="{ marginTop: '10px',width: '214.07px', height: '57.86px', top: '23.83px', left: '1px' , borderRadius: '5.14px',position: 'absolute' }" />
          
          
                  <div class="credit-card-rectangle" :style="{ width: '7.77px', height: '7.77px', top: '110.55px', left: '5px', backgroundColor: activeButtonColor,borderRadius: '7.77px',position: 'absolute'}"></div>
                      <p class="credit-card-text" :style="{ width: '82.38px', height: '11px', top: '100px', left: '20px',  fontSize: '9.33px', fontWeight: 700, lineHeight: '11.19px', textAlign: 'left', color: activeButtonColor, position: 'absolute', }">Credit Card</p>

            <div class="detail-form" :style="{ width: '214.07px', height: '204.43px', top: '140.31px', gap: '20.29px', borderRadius: '9.64px', position: 'absolute'}">
                <!-- Images -->
                  <img src="@/assets/section5/email.svg" alt="Image 1" class="detail-image" :style="{ width: '214px', height: '39px', position: 'absolute',top : '0px',left: '-3px' }" />
                  <img src="@/assets/section5/details.svg" alt="Image 2" class="detail-image" :style="{ width: '214px', height: '65px', gap: '10px',position: 'absolute',top: '45px' }" />
                  <img src="@/assets/section5/name.svg" alt="Image 3" class="detail-image" :style="{ width: '214px', height: '39px', gap: '10px',position: 'absolute',top: '115px' }" />
               <!-- Pay Now button -->
                 <button class="pay-now-button" :style="{backgroundColor: activeButtonColor, width: '214.07px', height: '29.57px', top: '165.85px', borderRadius: '4.5px', position: 'absolute', border: 'none', left: '1.5px', textAlign: 'center' }">Pay Now</button>
             </div>
                <div class="payment-method" :style="{ width: '214.07px', height: '27px', top: '365.36px', gap: '0px', borderRadius: '4.5px', backgroundColor: '#082C34',position: 'absolute'}">
                  <div class="bullet1" :style="{ width: '7.77px', height: '7.77px', border: '1px solid' ,borderColor: activeButtonColor, borderRadius: '7.77px', position: 'absolute', top: '32%', left: '5%' }"></div>
                  <span style="width: 108px; height: 11px; top: 8.5px; left: 25.18px;  font-size: 9px; font-weight: 700; line-height: 10.8px; text-align: left; color: white; position: absolute;">PayPal</span>

                </div>
              <!-- Payment Method 2 -->
                <div class="payment-method" :style="{ width: '214.07px', height: '27px', top: '400.36px',  gap: '0px', borderRadius: '4.5px', backgroundColor: '#082C34',position: 'absolute' }">
                  <div class="bullet1" :style="{ width: '7.77px', height: '7.77px', border: '1px solid' ,borderColor: activeButtonColor, borderRadius: '7.77px', position: 'absolute', top: '32%', left: '5%' }"></div>
                  <span style="width: 108px; height: 11px; top: 8.5px; left: 25.18px; font-size: 9px; font-weight: 700; line-height: 10.8px; text-align: left; color: white; position: absolute;">Sofort</span>

                </div>
        </div>

      </div>
      <div class="additional-buttons">
      <button class="button1" :class="{ active: activeButton === 1 }" @click="activateButton(1)"></button>
      <button class="button2" :class="{ active: activeButton === 2 }" @click="activateButton(2)"></button>
      <button class="button3" :class="{ active: activeButton === 3 }" @click="activateButton(3)"></button>
      <button class="button4" :class="{ active: activeButton === 4 }" @click="activateButton(4)"></button>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'section5',
  data() {
    return {
      activeButton: 2, // Default active button is button 2
      activeButtonColor: '#B0A3FF' // Default background color for button 2
    };
  },

  methods: {
    activateButton(buttonIndex) {
      this.activeButton = buttonIndex;
      // Set background color based on active button
      if (buttonIndex === 1) {
        this.activeButtonColor = '#7CDDAE';
      } else if (buttonIndex === 2) {
        this.activeButtonColor = '#B0A3FF';
      } else if (buttonIndex === 3) {
        this.activeButtonColor = '#F8B968';
      } else if (buttonIndex === 4) {
        this.activeButtonColor = '#CD176E';
      }
    },

    getVectorSrc() {
      // Determine the SVG file based on the active button
      if (this.activeButton === 3) {
        return "@/assets/Vector1 copy.svg";
      } else {
        return "@/assets/Vector1.svg";
      }
    }
  }
};
</script>


<style scoped>

.black-fill {
  fill: black;
}

.pay-now-button {
  
font-weight: 900;
font-family: 'Ginka', sans-serif;
color: rgb(2, 33, 40);
font-size: 10.29px;
}
.section5 {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;


}

.box1 {
  text-align: center;
  justify-content: center;
  position: relative;
}

.button {
  width: 144px;
  height: 43px;
  gap: 10px;
  border: none;
  border-radius: 66px;
  font-family: 'Gink', sans-serif;
  font-size: 16px;
  font-weight: 700;
  line-height: 19.2px;
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
  font-size: 50px;
}

.paragraph {
  opacity: 50%;
  font-size: 18px;
  line-height: 27px;
}



.main-box {
  position: relative;
  width: 800.49px;
  height: 505.72px;
  top: 81.6px;
  left: 166.32px;
  border-radius: 28.9px;
  border: #B0A3FF 1.55px solid;
}

.order-summary-box {
  position: relative;
  width: 317.09px;
  height: 489.62px;
  top: 8.05px;
  left: 8.55px;
  gap: 0;
  border-radius: 20.23px;
  background: #B0A3FF;
  transition: background-color 0.3s ease; /* Transition for background color */

}

.eur-20 {
  width: 194px;
  height: 155px;
  position: absolute;
  top: 0;
  left: 0;
}

.text-20 {
  width: 168px;
  height: 155px;
  top: 11.66px;
  left: 25.43px;
  font-family: 'Ginka', sans-serif;
  font-size: 129.03px;
  font-weight: 700;
  line-height: 154.84px;
  text-align: left;
  color: white;
  position: absolute;
}

.text-eur {
  width: 32px;
  height: 19px;
  left: 167.58px;
  top: 41.06px;
  font-family: 'Ginka', sans-serif;
  font-size: 15.48px;
  font-weight: 700;
  line-height: 18.58px;
  text-align: left;
  color: white;
  position: absolute;
}

.order-summary-title {
  width: 162.65px;
  height: 15px;
  top: 292.99px;
  left: 30.64px;
  font-size: 12.28px;
  font-family: 'GinkaBold', sans-serif;
  font-weight: 700;
  text-align: left;
  color: white;
}

.order-summary-text {
  width: 197.43px;
  height: 9px;
  top: 299.36px;
  left: 32.64px;
  opacity: 0.6;
  font-family: 'GinkaBook', sans-serif;
  font-size: 7.37px;
  font-weight: 400;
  text-align: left;
  color: white
}

.rect1, .rect2 {
  width: 114.9px;
  height: 6.99px;
  top: 80.62px;
  left: 109.12px;
  border-radius: 49.96px;
  opacity: 0.3px;
  position: absolute;
}

.rect1 {
  background-color: #E5EAE9;
  opacity: 0.3;
}

.rect2 {
  width: 68.32px;
  top: 70.11px;
  opacity: 0.3;
  background-color: #E5EAE9;
}
.additional-buttons {
  display: flex;
  gap: 18.65px;
  width: 253.36px;
  height: 32.64px;
  top: 138.84px;
  left: 469.32px;
  position: relative;

}

.button1, .button3, .button4 {
  width: 32.64px;
  height: 32.64px;
  border-radius: 32.25px;
  opacity: 0.4;
  border: none;
  transition: all 0.3s ease; /* Transition for all button properties */

}

.button1 {
  background: #7CDDAE;
}

.button2 {
  width: 99.48px;
  height: 32.64px;
  background: #B0A3FF;
  border-radius: 32.25px;
  border: none;
}

.button3 {
  background: #F8B968;
}

.button4 {
  background: #CD176E;
}
.button1.active {
  opacity: 1;
  border-radius: 32.25px;
  width: 99.48px;
  height: 32.64px;
  background: #7CDDAE;

}

.button3.active {
  opacity: 1;
  border-radius: 32.25px;
  width: 99.48px;
  height: 32.64px;
  background: #F8B968;

}

.button4.active {
  opacity: 1;
  border-radius: 32.25px;
  width: 99.48px;
  height: 32.64px;
  background: #CD176E;

}

.additional-buttons .button2:not(.active) {
  width: 32.64px;
  height: 32.64px;
  border-radius: 32.25px;
  opacity: 0.4;
  border: none;
}





</style>
