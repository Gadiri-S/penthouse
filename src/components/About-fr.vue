<template>
  <div class="container">
    <h1>Notre processus</h1>

  <p>Tous les projets sur lesquels nous travaillons suivent des étapes bien précises pour s'assurer que votre projet vous convienne parfaitement!</p>

  <div class="process">

    <div class="container-package">

        <div class="package bronze one"> 

          <div class="number">
      <img src="../assets/one.png" class="number_icon" alt="">
    </div>
            <span class="title">Parlons de votre projet <img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail">Nous aurons tout d'abord une conversation téléphonique ou par vidéo-chat pour parler de votre entreprise et de vos besoins. Cette étape est cruciale tout aussi bien pour vous que pour nous car elle nous permettra de clarifier la stratégie à employer pour faire grandir votre entreprise. C'est un premier contact donc vous aurez tout le temps de réfléchir aux spécificités de votre projet et de poser toutes les questions qui vous traverseront l'esprit.
</span>
  </div> 
             <div class="pic" v-motion-fade-visible>  <img src="../assets/pa.png" alt="" class="test"  ></div>

  </div>

<div class="container-package">
   <img src="../assets/ka.png" alt="" class="test" v-motion-fade-visible >

         <div class="package bronze two">

                   <div class="number">
      <img src="../assets/two.png" class="number_icon" alt="">
    </div>
            <span class="title">Intéressons nous aux spécificités! <img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail"> Nous déterminerons ensemble le bouquet qui vous convient le mieux. Nous déterminerons aussi les particularités de votre site notamment le style et les fonctionnalités. Bien que vous serez chargé de nous fournir le contenu textuel du site, vous aurez toujours le temps de le rédiger. Une fois que le cahier des charges est validé et signé, vous nous paierez un accompote de 30% du coût total du projet.
</span>
  </div>
</div>


<div class="container-package">

           <div class="package bronze three">
                          <div class="number">
   <div>  <img src="../assets/three.png" class="number_icon" alt=""></div> 
    </div>
            <span class="title">Développement! <img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail">Il est maintenant temps de construire votre site. En fonction de la taille du projet et la vitesse à laquelle vous nous fournirez les éléments devant composer le site (texte, images si vous voulez utiliser les votres), le procédé peut prendre en moyenne entre 3 et 4 semaines.</span>
            
  </div>
   <img src="../assets/pop.png" alt="" class="test" v-motion-fade-visible >

</div>


<div class="container-package">
     <img src="../assets/a.png" alt="" class="test" v-motion-fade-visible >

             <div class="package bronze four">
                                            <div class="number">
      <img src="../assets/four.png" class="number_icon" alt="">
    </div>
            <span class="title">Déploiement en ligne <img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail">Une fois que le projet est validé et que vous êtes satisfait de votre nouveau site, il est temps de le mettre en ligne. Le montant restant de la prestation sera versé à ce moment.
</span>
  </div>

  </div>

  <div class="container-package">
             <div class="package bronze five">
                               <div class="number">
      <img src="../assets/five.png" class="number_icon" alt="">
    </div>
          
            <span class="title"><img src="../assets/star.png" class="star" alt="">Brillez!<img src="../assets/star.png" class="star" alt=""></span>
            <span class="detail">            Il est maintenant temps pour votre entreprise d'atteindre de nouveaux sommets! Que vous souscriviez à un bouquet de maintenance ou que vous decidiez de continuer votre aventure seul, votre entreprise a désormais tout pour démontrer la qualité de vos services et votre profesionnalisme!
</span>
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
.one{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/pa.png');
}
.two{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/ka.png');
}
.three{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/ma.png');
}
.four{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/a.png');
}
.five{     background: linear-gradient(rgba(0, 0, 0, 0.515),rgba(0, 0, 0, 0.515)),url('../assets/bpr.png');
}

}

</style>