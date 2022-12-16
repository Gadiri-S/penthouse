<template>
  <div class="container">
    <h1>Our process</h1>

    <p>Every project that we manage follows a very specific process to ensure the best experience for the customer and make sure that nothing has been left out!</p>
  

  <div class="process">

    <div class="container-package">

        <div class="package bronze one"> 

          <div class="number">
      <img src="../assets/one.png" class="number_icon" alt="">
    </div>
            <span class="title">First: Let's talk about your project <img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail">We will first have a phone conversation or zoom call to talk about your business and what you need. This stage is crucial for both us as it will clarify our strategy to help your business grow through your website. It's a first contact so you will still have the time to make up your mind if you're not sure about the specifics of what you need or if you have some questions.</span>
            
  </div> 
             <div class="pic" v-motion-fade-visible>  <img src="../assets/pa.png" alt="" class="test"  ></div>

  </div>

<div class="container-package">
   <img src="../assets/ka.png" alt="" class="test" v-motion-fade-visible >

         <div class="package bronze two">

                   <div class="number">
      <img src="../assets/two.png" class="number_icon" alt="">
    </div>
            <span class="title">Let's get into the details! <img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail">Now is time to get into the details of your website. We will establish together what is the best package for your business. We will also get into the specifics concerning the style of the website, the content and the functionalities. Although you will have to provide the content you want us to write, you'll still have time to think about it while we build the website for you. Once everything is agreed we will send you a quote with an account of 30% the total price of the project.</span>
            
  </div>
</div>


<div class="container-package">

           <div class="package bronze three">
                          <div class="number">
   <div>  <img src="../assets/three.png" class="number_icon" alt=""></div> 
    </div>
            <span class="title">Development! <img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail">Time for us to build your website. Depending on the size of the project and how fast your provide the necessary material (text, images if you want us to use your own), the process can take on average between 3 to 4 weeks.</span>
            
  </div>
   <img src="../assets/pop.png" alt="" class="test" v-motion-fade-visible >

</div>


<div class="container-package">
     <img src="../assets/a.png" alt="" class="test" v-motion-fade-visible >

             <div class="package bronze five">
                                            <div class="number">
      <img src="../assets/four.png" class="number_icon" alt="">
    </div>
            <span class="title">Deployment online <img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail">Once everything is agreed and that you are happy with your new website, it's time for us to host it online. The remaining of the fare will be paid at that moment.</span>
            
  </div>

  </div>

  <div class="container-package">
             <div class="package bronze five">
                               <div class="number">
      <img src="../assets/five.png" class="number_icon" alt="">
    </div>
          
            <span class="title"><img src="../assets/star.png" class="star" alt="">Shine!<img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail">Now it's time for your business to reach new heights. Rather you subscribed to a maintenance package or decided to handle the rest yourself, your business has everything it needs to showcase how great is your company and the services you provide!</span>
            
  </div>
     <img src="../assets/bpr.png"  alt="" class="test" v-motion-fade-visible >


</div>
  </div>
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

.process{
  display: flex;
  flex-direction: column;
}

.number_icon{
  height: 40px;
}
h1{
    font-size: 45px;
    padding: 20px 0;
}
p{
    font-size: 25px;
}
.container-package{
  display: flex;
  align-items: center


}
.package{
    display: flex;
    flex-direction: column;
    width: 400px;
    padding: 15px;
    border-radius: 15px;
    margin: 25px auto;

    .title{
        font-size: 25px;
        font-weight: 600;
        padding:  25px 10%;
        
    }
    .detail{
        font-weight: 500;
        font-size: 20px;
                padding: 2% 10%;

    }
}
.bronze{
     background:url('../assets/back.png');
     background-size:contain;
     color: white;
     background-color: transparent;
     box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
  transition: .4s ease-in-out;
  position: relative;
  top: 0;

&:hover{
  transition: .4s ease-in-out;
     color:#00009e;
     background-color: white;
     cursor: pointer;
       top: 10px;

}
}
.one,.three,.five{
    box-shadow: rgba(240, 46, 170, 0.4) -5px 5px, rgba(240, 46, 170, 0.3) -10px 10px, rgba(240, 46, 170, 0.2) -15px 15px, rgba(240, 46, 170, 0.1) -20px 20px, rgba(240, 46, 170, 0.05) -25px 25px;

&:hover{
                box-shadow: rgba(255, 196, 0, 0.4) -5px 5px, rgba(255, 196, 0, 0.3) -10px 10px, rgba(255, 196, 0, 0.2) -15px 15px, rgba(255, 196, 0, 0.1) -20px 20px, rgba(255, 196, 0, 0.05) -25px 25px;
transition: .4s ease-in-out;
}
}
.two,.four{
    box-shadow: rgba(240, 46, 170, 0.4) 5px 5px, rgba(240, 46, 170, 0.3) 10px 10px, rgba(240, 46, 170, 0.2) 15px 15px, rgba(240, 46, 170, 0.1) 20px 20px, rgba(240, 46, 170, 0.05) 25px 25px; 
&:hover{
    box-shadow: rgba(255, 196, 0, 0.4) 5px 5px, rgba(255, 196, 0, 0.3) 10px 10px, rgba(255, 196, 0, 0.2) 15px 15px, rgba(255, 196, 0, 0.1) 20px 20px, rgba(255, 196, 0, 0.05) 25px 25px; 
transition: .4s ease-in-out;
}
}

.pic{

}
.test{
  height: 340px;
}

.star{
  height: 15px;
}

@media (max-width:1100px) {

  .package{
    display: flex;
    flex-direction: column;
    width: 350px;
    padding: 15px;
    border-radius: 15px;
    margin: 25px auto;

    .title{
        font-size: 20px;
        font-weight: 600;
        padding:  20px;
    }
    .detail{
        font-weight: 500;
        font-size: 18px;
                padding: 2% 10%;

    }
}
  
  .test{
    height: 200px;
  }
}

@media (max-width:800px) {

  .package{
    display: flex;
    flex-direction: column;
    width: 80%;
    padding: 15px;
    border-radius: 15px;
    margin: 25px auto;

    .title{
        font-size: 20px;
        font-weight: 600;
        padding:  20px;
    }
    .detail{
        font-weight: 500;
        font-size: 18px;
                padding: 2%;

    }
}
  
  .test{
    display: none;
  }

  .bronze{
     background-size:cover;
     background-repeat: no-repeat;
     color: white;
     box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;

     &:hover{
  transition: .4s ease-in-out;
     color:inherit;
     background-color: inherit;
     cursor: pointer;
       top: 10px;

}
}
.one{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/ma.png');
}
.two{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/pa.png');
}
.three{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/ta.png');
}
.four{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/r.png');
}
.five{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/pa.png');
}
.six{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/a.png');
}
}

</style>