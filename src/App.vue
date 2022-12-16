<template>
<div>

  <router-view/>
  </div>
</template>

<script>

export default {
   
}
</script>
<style lang="scss">



*{
  padding: 0;
  margin: 0;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  font-family: 'Raleway', sans-serif;
  color:white;

  h1{
  font-family: 'Poppins', sans-serif;

  }

}



    button{
        font-size: 20px;
        padding: 10px;
        border-radius: 5px;
        background: rgb(71, 71, 163);
        border: 1px solid rgb(71, 71, 163);
        color:white;
        font-weight: 600;
        font-family: 'Raleway', sans-serif;
              cursor:pointer;   
              transition: .4s ease-in-out;
              
              &:hover{
        background: rgb(255, 174, 0);
                border: 1px solid rgb(255, 174, 0);;

                              transition: .4s ease-in-out;

              }
              
              }

button,textarea,input{
    font-family: 'Raleway', sans-serif;

}

a{
  text-decoration: none;

  &:visited{
    color: inherit;
  }
}





@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Raleway:wght@400;500;600;700;800;900&display=swap');
</style>
