<template>
  <div class="container">
    <h1>Why a website and what to look for?</h1>


    <div class="content">
       <div class="container-picture" v-motion-roll-visible-left><img src="../assets/popa.png" alt="" class="pic"></div> 
        <h2><img src="../assets/star.png" class="star" alt="">Your website should be a solution, not a commodity<img src="../assets/star.png" class="star" alt=""></h2>
    </div>

    <p>We strongly believe that a website is first and foremost a solution. Often time, it can be easy to see the later as an accessory but it should always answer to a very specific need you have.</p>
 <p>The best website for you is the website that allows you to showcase your skills, your profesionnalism, you services but also your style and identity!</p>
    <h2 class="questions_title">Key advantages to a website</h2>

  <ul class="advantages">
        <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">Your business will grow</li>
      <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">A website adds legitimacy to your business</li>
    <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">You will be able to display your skills and services</li>
    <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">New customers will now easily be able to find you</li>
    <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">Through contact forms, customers will be able to reach you quickly</li>

  
  
  </ul>

  <h2 class="questions_title">Few questions to ask yourself</h2>
  <ul class="questions">
    <li v-motion-fade-visible-once>Do I want my business or organization to grow?</li>
    <li v-motion-fade-visible-once>Do I believe that my business or organization deserves more visibility?</li>
    <li v-motion-fade-visible-once>Do I believe that the public would benefit from the products or services I provide?</li>
    <li v-motion-fade-visible-once>Do I need or want to make a great first impression to potential clients or customers?</li>
    <li v-motion-fade-visible-once>Do I want to be able to see how many people visit my website and when?</li>
  </ul>
  <h2 class="questions_title" v-motion-fade-visible>Yes? Then don't wait any longer and check our packages!</h2>
  </div>
  
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.container{
  background-color: #00009e;
 background-repeat: no-repeat;
  background-position: left; 
    background-size: contain;

 color: white;
 min-height: 100vh;
 padding: 2%;
}

.content{
  display: flex;
  align-items: center;
}


h1{
    font-size: 45px;
    padding: 20px 0;
}
h2{
        font-size: 35px;
        width: 50%;
}
p{
    font-size: 25px;
}

.container-picture{
    width: 50%;
}
.pic{
    height: 400px;
}
.star{
    height: 15px;
}

.questions_title{
    width: 100%;
    margin: 25px auto;
}

ul{
width: 50%;
margin: 25px auto;
text-align: center;}

.advantages{
    list-style-type: none;
}
li{
    font-size:25px;
    margin: 5px 0;
    text-align:left;
}
</style>