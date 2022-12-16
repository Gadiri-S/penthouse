<template>
  <div class="container">
    <h1>Pourquoi un site web?</h1>


    <div class="content">
       <div class="container-picture" v-motion-roll-visible-left><img src="../assets/popa.png" alt="" class="pic"></div> 
              <div class="container-picture-mobile" v-motion-roll-visible-left><img src="../assets/popa.png" alt="" class="pic"></div> 

        <h2><img src="../assets/star.png" class="star" alt="">Votre site web doit être une solution, non un accessoire<img src="../assets/star.png" class="star" alt=""></h2>
    </div>

    <p>Nous avons la conviction qu'un site web est avant tout une solution. Il peut souvent être tentant de voir ce dernier comme un accessoire mais il doit toujours répondre à des besoins spécifiques que vous avez.</p>
 <p>    Le meilleur site pour vous est celui qui vous permet de démontrer vos compétences, votre profesionnalisme ainsi que vos services mais aussi votre style et votre identité!</p>
    <h2 class="questions_title">Les avantages clefs d'un site web</h2>
  <ul class="advantages">
        <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">Votre entreprise grandira</li>
      <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">Votre site ajoutera de la légitimité à votre entreprise</li>
    <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">Vous pourrez clairement et rapidement montrer vos services et vos compétences</li>
    <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">De nouveaux clients seront capables de vous trouver</li>
    <li v-motion-fade-visible-once><img src="../assets/star.png" class="star" alt="">Vos clients pourront rapidement et facilement vous contacter grâce au formulaire de contact</li>

  
  
  </ul>

  <h2 class="questions_title">Quelques questions à vous poser</h2>
  <ul class="questions">
    <li v-motion-fade-visible-once>Voulez vous voir votre entreprise ou organisation grandir?</li>
    <li v-motion-fade-visible-once>Pensez vous que votre entreprise ou organisation mérite une plus grande visibilité?</li>
    <li v-motion-fade-visible-once>Pensez vous que le public bénéficierai des produits et services que vous pourvoyez?</li>
    <li v-motion-fade-visible-once>Voulez vous faire une bonne première impression face à vos potentiels futurs clients ou partenaires?</li>
    <li v-motion-fade-visible-once>Voulez vous avoir de la visibilité sur l'impact qu'a votre site sur la toile?</li>
  </ul>
  <h2 class="questions_title" v-motion-fade-visible>Oui? Alors n'attendez plus une seule seconde et découvrez nos bouquets!</h2>
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

.container-picture-mobile{
  display: none;
}
.star{
    height: 15px;
}

.questions_title{
    width: 100%;
    margin: 25px auto;
}

ul{
width: 70%;
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

@media (max-width:900px) {

  .container{
    padding: 5%;
  }
  .content{
    flex-direction: column;
  }

  .container-picture{
    width: 100%;
}
h2{
        font-size: 25px;
        width: 100%;
        margin: 25px 0;
}

.advantages,.questions{
width: 100%;
margin: 7px auto;
text-align: center;
width: 95%;
}
.container-picture-mobile{
display: block;
}
.container-picture{
  display: none;
}
li{
  font-size:19px;
      margin: 25px auto;

}

.questions_title{
    margin: 25px auto;
}

p{
  font-size: 20px;
}

.pic{
  height: 350px;
}
}

</style>