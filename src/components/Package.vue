<template>
  <div class="container">
    <h1>Our packages</h1>

    <p>Our packages are tailored for businesses with different needs. We will help you choose the best offer based on your current and future aspirations. Remember that a cheaper package is not synonymous of lesser quality!</p>

    <div class="package-container">
        <div class="package bronze" v-motion-fade-visible-once>
            <span class="title">Bronze Package</span>
            <span class="detail">Personalized website ideal for small businesses who are just getting started and who are looking for an online presence.</span>
                <ul>
                    <li>Custom website</li>
                    <li>Photo sourcing</li>
                    <li>Social media integration</li>
                    <li>Google Maps</li>
                    <li>Contact form</li>
                    <li>One year hosting</li>
                    <li>Mobile responsive</li>
                    <li>Accessibility</li>
                    <li><strong>5 pages included*</strong> <br>                     <span class="page">150euros per additional page*</span>   
</li>
                    </ul>

                    <span class="price">1500€</span>   
        </div>
                <div class="package silver" v-motion-fade-visible-once>
                     <span class="title">Silver Package</span>
            <span class="detail">Perfect for businesses who are trying to grow their brand. You'll be able to fully showcase your business and the services you offer with a website tailored just for you.</span>
               
               
                   <ul>
                    <li>Custom website</li>
                    <li>Photo sourcing</li>
                    <li>Social media integration</li>
                    <li>Google Maps</li>
                    <li>Contact form</li>
                    <li>One year hosting</li>
                    <li>Mobile responsive</li>
                    <li>SEO</li>
                    <li>Accessibility</li>
                    <li>Database</li>
                    <li>Customized content</li>
                    <li>Blog</li>
                    <li>Admin dashboard</li>
                    <li><strong>10 pages included*</strong> <br>                                         <span class="page">150euros per additional page*</span>   
</li>
                    </ul>

                    <span class="price">3500€</span>  

                </div>
                        <div class="package gold" v-motion-fade-visible-once>
                                        <span class="title">Gold Package</span>
            <span class="detail">Bring your business to the next level! Ideal for E-commerce stores and businesses who want to sell their products online.</span>

   
                   <ul>
                    <li>Custom website</li>
                    <li>Photo sourcing</li>
                    <li>Social media integration</li>
                    <li>Google Maps</li>
                    <li>Contact form</li>
                    <li>One year hosting</li>
                    <li>Mobile responsive</li>
                    <li>Accessibility</li>
                    <li>Database</li>
                    <li>Customized content</li>
                    <li>Blog</li>
                    <li>Admin dashboard</li>
                    <li>E-Commerce solution</li>
                    <li>User interface</li>
                    <li>SEO</li>
                    <li>Google Analytics</li>
                    <li><strong>10 pages included*</strong><br>
                                                            <span class="page">150euros per additional page*</span>   

                    </li>
                    </ul>

                    <span class="price">5000€</span> 

                        </div>

    </div>
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
    padding: 2%;
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
p{
    font-size: 25px;
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
transition: .4s ease-in-out;
  top: 0;
  position: relative;


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
     height: 450px;

}
.silver{
     background:linear-gradient(rgba(0, 0, 0, 0.836),rgba(0, 0, 0, 0.836)),url('../assets/po.png');
     color: rgb(255, 255, 255);
     height: 580px;

}
.gold{
         background:linear-gradient(rgba(0, 0, 0, 0.747),rgba(0, 0, 0, 0.671)),url('../assets/b.jpg');

}

strong{
    color:#ffbb00 ;
}
</style>