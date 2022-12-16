<template>
  <div class="container">
   <h1> Contactez nous! </h1>
 <div v-if="isFormCorrect">
<div class="success">
  <span>Votre message a bien été envoyé. <br><br><br>Merci! </span>
<span class="icon">  <font-awesome-icon  icon="far fa-check-circle" /></span>

</div>
</div>
<div v-else>
  <form ref="form" @submit.prevent="handleSubmit">
        <input type="text" placeholder="Prénom*" v-model="firstname" name='firstname'  @blur="v$.firstname.$touch" required>
          <div v-if="v$.firstname.$error" class="error">Champ obligatoire.</div>
        
        <input type="text" placeholder="Nom de famille*" v-model="lastname" name='lastname'  @blur="v$.lastname.$touch" required> 
                  <div v-if="v$.lastname.$error" class="error">Champ obligatoire.</div>
                <input type="text" placeholder="Nom de l'entreprise*" v-model="business" name='business'  @blur="v$.business.$touch" required> 
                  <div v-if="v$.lastname.$error" class="error">Champ obligatoire.</div>
        <input type="email" placeholder="Email*" v-model="email" name='email' @blur="v$.email.$touch" required>
                  <div v-if="v$.email.$error" class="error">Veuillez entrer une addresse mail valide.</div>
       
        <input type="tel" placeholder="Numéeo de téléphone*" v-model="tel" name='tel'  @blur="v$.tel.$touch" required>
                  <div v-if="v$.tel.$error" class="error">Veuillez entrer un numéeo de téléphone valide.</div>
        
       
        <textarea name="message" id="message" cols="30" rows="10" placeholder="Your message *" v-model="message" @blur="v$.message.$touch" required></textarea>
                  <div v-if="v$.message.$error" class="error">Champ obligatoire.</div>

        <button @click="send">Envoyer</button>

    </form>  </div>
  </div>
</template>

<script>
import { useVuelidate } from '@vuelidate/core'
import { required, email, alpha, numeric, alphaNum } from '@vuelidate/validators'
export default {
setup () {
    return { v$: useVuelidate() }
  },
  data () {
    return {
      firstname: '',
      lastname: '',
      business:'',
        email: '',
        tel:'',
        message:'',
        isFormCorrect:"",
        submitted: false

    }
  },
  validations () {
    return {
      firstname: { required }, // Matches this.firstName
      lastname: { required }, // Matches this.lastName
            business: { required }, // Matches this.lastName

        email: { required }, // Matches this.contact.email
      message: { required }, // Matches this.lastName
      tel: { numeric }, // Matches this.lastName
            tel: { required }, // Matches this.lastName


  
    }
  },
    created() {
            setTimeout(() => this.isFormCorrect = false, 1000)
        },
   methods: {
           async send() {
                this.submitted = true;
const isFormCorrect = await this.v$.$validate();
this.isFormCorrect = isFormCorrect

/*if (isFormCorrect==true) {
emailjs.sendForm('service_qx8ql38', 'template_wlflq6g', this.$refs.form, 'iMSRNYA0xKflKPitU')
        .then((result) => {
            console.log('SUCCESS!', result.text);
        }, (error) => {
            console.log('FAILED...', error.text);
        });}


    
*/


      // you can show some extra alert to the user or just leave the each field to show it's `$errors`.
      if (!isFormCorrect) return console.log('error')
            }
        }
}
</script>

<style lang="scss" scoped>
.container{
    min-height: 100vh;
    background: #260081;
    padding: 2%;
}

h1{
    font-size: 45px;
    padding: 20px 0;
}
form{
    display: flex;
    flex-direction: column;
    width: 700px;
    margin: 25px auto;
    padding: 10px;
      background:url('../assets/back.png');
     background-size:contain;
     
    
    input,textarea{
        border-radius: 5px;
        border: none;
box-shadow: rgba(106, 148, 255, 0.25) 0px 4px 8px -2px, rgba(111, 169, 255, 0.08) 0px 0px 0px 1px;
  font-size:20px;
    padding: 6px 6px 6px 10px;
    margin: 5px auto;
    width: 80%;
background-color:transparent;
     color: white;

    }

    button{
        width: 80%;
        margin: 10px auto;
    }

    ::placeholder{
        color: rgb(255, 255, 255);
    }
}

.error{
    color: red;
}
.success{
  display: flex;
  flex-direction: column;
  height: 300px;
  width: 450px;
  border-radius: 15px;
    background: rgb(255, 255, 255);
    color: rgb(0, 47, 255);
    margin: 25px auto;

  span{
    font-size: 25px;
    color: rgb(0, 47, 255);
        margin: 25px auto;

  }
  .icon{
     font-size: 45px;
    color: rgb(0, 255, 179);
    margin: 25px auto;
  }
}

@media (max-width:900px) {
    form{
        width: 80%;
    }
}
</style>