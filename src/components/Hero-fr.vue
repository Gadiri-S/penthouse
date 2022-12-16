<template>
  <div class="hero-container">
    <HeaderFr/>


    <div class="container" v-motion
    :initial="{ opacity: 0, y: 100 }"
  :enter="{
    y: 0,
    opacity: 1,
    transition: {
      duration: 900,
      type: 'keyframes',
      ease: 'easeIn',
    },
  }">
      <div class="text">
<h1>penthouse web solutions <img src="../assets/star.png" class="star" alt=""></h1><img src="../assets/star.png" class="star" alt="">
<span>Des solutions web<br>pour accompagner votre entreprise</span>

<div><button  @click="nav(contact[0].id)">Nos bouquets</button></div>
</div>
      <div class="picture">
        <div class="pic1">
                    <img src="../assets/r.png" class="big" alt="">

        </div>
        
     
</div>


</div>

  </div>
</template>

<script>


import HeaderFr from '@/components/Header-fr.vue'

export default {
  name: "Hero",
  components: {
    HeaderFr
  },

  data() {
    return {
image:"",
products:"",
selected:false,
     contact: [
   {
id: 'contact'}],

    }
  
  }, 

  methods:{


       nav(id) {

        const position = document.getElementById(id).offsetTop;
          // smooth scroll
         window.scrollTo({ top: position, behavior: "smooth" });  
    },

  }

}
</script>

<style lang="scss" scoped>

.container{
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    padding: 2%;
    overflow-x: hidden;
}

.hero-container {
  background: linear-gradient(rgba(21, 21, 87, 0.829),rgba(21, 21, 87, 0.836)),url('../assets/co.png');
  background-color: #00009e;
 background-repeat: no-repeat;
  background-position: left; 
    background-size: contain;

 color: white;
 min-height: 100vh;
}

.text {
    text-align: left;
    width: 50%;




    h1 {
            font-size: 70px;
            font-weight: 600;
            margin-bottom: 25px;
            text-transform: uppercase;
            letter-spacing: 2.5px;

            }

            span{
              font-size: 35px;
            }


            button{
              font-size: 25px;
              border: 1px solid white;
              border-radius: 25px;
              background: transparent;
              color: white;
              padding: 10px 25px;
              margin: 25px auto;
              font-family: 'Raleway', sans-serif;
              cursor:pointer;
                  transition: .5s ease-in-out;


              &:hover{
            background: rgb(255, 174, 0);
    border: 1px solid transparent;
    cursor: pointer;
    transition: .5s ease-in-out;
    color:  #250f63;;
}
            }

    
}

           .picture{
            display: flex;
           }

.star{
    height: 30px;
}

.big{
  height: 500px;
  width: 400px;
  object-fit: cover;
  border-radius: 20px;
  padding: 10px;
}


  @keyframes moveleft {

        0% {
            transform: translateX(800px);
        }
        100% {
            transform: translateX(0px);
    
        }
    }
      @keyframes moveright {

        0% {
            transform: translateX(-800px);
        }
        100% {
            transform: translateX(0px);
    
        }
    }




@media (max-width:900px) {

  .container{
    flex-direction: column;
  }
  .text {
    margin: 2% 0 0 0;
    padding: 0;
    text-align: center;
    width: 100%;

    h1 {
    font-size: 50px;
  }

  span{
    font-size: 30px;
  }
  }

 
 
 .container-small{
  display: flex;
    flex-direction: column;
 }
}

@media (max-width:700px) {
   .picture{
    flex-direction: column;
  }
   .container-small{
    flex-direction: row;
 }
}
@media (max-width:600px) {
   .picture{
    flex-direction: column;
  }
   .container-small{
    flex-direction: column;
 }
}


</style>