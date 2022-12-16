<template>
  <div class="container">
    <h1>Nos bouquets</h1>

    <div class="package-container">
        <div class="package bronze">
            <span class="title">Bouquet Bronze</span>
            <span class="detail">Site personnalisé. Idéal pour les petites entreprises qui viennent de débuter et qui chercher à dispose d'une présence sur internet.</span>
                <ul>
                    <li>Site personnalisé</li>
                    <li>Photos</li>
                    <li>Intégration des réseaux sociaux</li>
                    <li>Google Maps</li>
                    <li>Formulaire de contact</li>
                    <li>Une année d'hébergement sur un serveur</li>
                    <li>Adaptation aux petits et moyens écrans</li>
                    <li>Accessibilité pour les personnes souffrant de handicap</li>
                    <li><strong>5 pages incluses*</strong> <br>                     <span class="page">150euros par page additionnelle*</span>   
</li>
                    </ul>

                    <span class="price">1500€</span>   
        </div>
                <div class="package silver">
                     <span class="title">Bouquet Argent</span>
            <span class="detail">Parfait pour les entreprises qui veulent s'étendre. Vous serez en mesure de démontrer toutes vos qualités et votre profesionnalisme avec un site fait juste pour vous.</span>
               
               
                   <ul>
                    <li>Site personnalisé</li>
                    <li>Photos</li>
                    <li>Intégration des réseaux sociaux</li>
                    <li>Google Maps</li>
                    <li>Formulaire de contact</li>
                    <li>Une année d'hébergement sur un serveur</li>
                    <li>Adaptation aux petits et moyens écrans</li>
                    <li>Accessibilité pour les personnes souffrant de handicap</li>
                    <li>SEO</li>
                    <li>Contenu dynamique customisable</li>
                    <li>Base de données</li>
                    <li>Blog</li>
                    <li>Page administrateur</li>
                    <li><strong>10 pages incluses*</strong> <br>                                        <span class="page">150euros par page additionnelle*</span>  
</li>
                    </ul>

                    <span class="price">3500€</span>  

                </div>
                        <div class="package gold">
                                        <span class="title">Bouquet Or</span>
            <span class="detail">Propulsez votre entreprise au sommet! Ideal pour le E-Commerce et les entreprises qui souhaitent vendre leurs produits et services en ligne.</span>

   
                   <ul>
                     <li>Site personnalisé</li>
                    <li>Photos</li>
                    <li>Intégration des réseaux sociaux</li>
                    <li>Google Maps</li>
                    <li>Formulaire de contact</li>
                    <li>Une année d'hébergement sur un serveur</li>
                    <li>Adaptation aux petits et moyens écrans</li>
                    <li>Accessibilité pour les personnes souffrant de handicap</li>
                    <li>Contenu dynamique customisable</li>
                    <li>Base de données</li>
                    <li>Blog</li>
                    <li>Page administrateur</li>
                    <li>Solutions E-Commerce</li>
                    <li>Interface utilisateur</li>
                    <li>SEO</li>
                    <li>Google Analytics</li>
                                       <li><strong>10 pages incluses*</strong> <br>                                         <span class="page">150euros par page additionnelle*</span>   
</li>
                    </ul>

                    <span class="price">5000€</span> 

                        </div>


    </div>

    <h1>Nos bouquets de maintenance</h1>
  </div>
</template>

<script>
export default {

}
</script>

<style lang='scss' scoped>
.container{
    min-height: 100vh;
    background: #260081;
}
.package-container{
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    margin-top: 25px;
}

h1{
    font-size: 45px;
        padding: 20px 0;

}
.package{
    display: flex;
    flex-direction: column;
    min-height: 450px;
    width: 350px;
    padding: 15px;
    border-radius: 15px;
    color: white;
    margin: 25px auto;
  top: 0;
  position: relative;
transition: .4s ease-in-out;


        &:hover{
cursor: pointer;
transition: .4s ease-in-out;
  top: 15px;

    }

    .title{
        font-size: 25px;
        font-weight: 600;
        padding: 25px 0;
    }
    .detail{
        font-weight: 500;
        font-size: 20px;
    }
}
.page{
    font-size: 12px;
}
ul{
    text-align: left;
    padding: 15px;
          font-weight: 500;
        font-size: 18px;
}

.price{
    color: #ffbb00;
    font-size: 35px;
    font-weight: 700;
}

.bronze{
     background:linear-gradient(rgba(0, 0, 0, 0.747),rgba(0, 0, 0, 0.671)),url('../assets/c.jpg');
     height: 520px;

}
.silver{
     background:linear-gradient(rgba(0, 0, 0, 0.836),rgba(0, 0, 0, 0.836)),url('../assets/po.png');
     color: rgb(255, 255, 255);
     height: 650px;

}
.gold{
         background:linear-gradient(rgba(0, 0, 0, 0.747),rgba(0, 0, 0, 0.671)),url('../assets/b.jpg');

}

strong{
    color:#ffbb00 ;
}
</style>