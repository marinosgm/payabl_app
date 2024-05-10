<template>
    <div class="section1">
      <div class="left-section">
        <div class="box">
          <h1>Welcome to payabl.
            an <b>omniverse</b> of payments.
          </h1>
          <p>
            Game-changing financial solutions for businesses with their eyes on
            global domination. Explore the endless payments possibilities with
            payabl. and level-up your business today.
          </p>
          <div class="buttons">
            <button class="lets-talk">Let's talk</button>
            <button class="whats-new">What's new?</button>
          </div>
        </div>
      </div>
      <div class="right-section">
        <div class="image-container">
            <img src="@/assets/section1/img1.svg" alt="Logo">
        </div>
      </div>
    </div>
  </template>
  
  <script>

  export default {
    name: 'Section1',
  };


  </script>
  
  <style scoped>
 


.section1 {
    display: flex;
    justify-content: space-between;
    background-color: --primary-color;
    padding: 200px;
    margin-top: 100px;
  }
  
  .left-section {
    flex: 1;
    display: flex;
    align-items: center;
    font-family:Gink, sans-serif;
    padding: 0px 15px;
    background-color: --primary-color;

    
    
    
  }
  
  .right-section {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: right;
    align-items: flex-end;
    width: 100%;
    position:relative;
    max-width: 100%;right:300px;
  }
  
  .box {
    width: 848px;
    height: 366px;
    padding: 0px 15px;
    width: 100%; /* Adjust the box size to get smaller when shrinking the window */
    height: 100%; /* Adjust the box size to get smaller when shrinking the window */
    background-color: --primary-color;


  }
  
  h1 {
    font-weight: 400;
    line-height: normal;
    font-size: 60px;
    margin:0px 0px 24px;
    color: #fff;
    font-family: 'GinkaLight', sans-serif; /* Apply the font-family Ginka */

  }
  
  p {
    font-size: 18px;
        margin: 24px 0;
        max-width: 703px;
        opacity: .5;
        color: #ffffff;
        font-family: 'GinkaLight', sans-serif; /* Apply the font-family Ginka */



  }
  
  .buttons {
    display: flex;
    gap: 10px;
    margin-top: 30px;
  }
  
  button.whats-new {
    padding: 0 24px;
  border: 2px solid #fff;
  border-radius: 12px;
  font-weight: 700;
  height: 43px;
  width: 151px;
  line-height: 39px;
  background-color: transparent;
  color: white;
  cursor: pointer;
  font-family: 'GinkaMedium', sans-serif; /* Apply the font-family Ginka */


  }

  .whats-new:hover {
    background-color: rgba(124, 221, 174, .3);

    -moz-transition: all .2s ease-in-out !important;
    transition: all .2s ease-in-out !important;

}

  .lets-talk {
    background-color: #7cddae;
  border: 2px solid #7cddae;
  border-radius: 12px;
  color: #022128;
  font-weight: 700;
  width: 120px;
  height: 43px;
  line-height: 39px;
  padding: 0 24px;
  text-align: center;
  font-family: 'GinkaMedium', sans-serif; /* Apply the font-family Ginka */
  }



  @media (max-width: 768px) {
        .section1 {
            flex-direction: column;
            padding: 20px;
        }

        .box, h1, p {
            width: 100%; /* Ensures full width usage on small screens */
        }

        h1 {
            font-size: 6vw; /* Larger font size for smaller screens */
        }

        p {
            font-size: 2.5vw;
        }

        .buttons {
            flex-direction: column;
            align-items: center;
        }

        button {
            width: 100%; /* Full width buttons for easier touch */
            margin-top: 10px;
        }

        .image-container {
            width: 80%; /* Make the image container responsive */
            margin: auto; /* Center align the image */
        }
    }

.image-container {
width: 400px;
height: 778.8px;
top: 146.56px;

}

  </style>