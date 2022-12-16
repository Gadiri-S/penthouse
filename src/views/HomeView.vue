<template>
  <div class="home">

    <Hero/>
    <Why/>
        <Package/>
<About/>
<Contact/>

  </div>
</template>

<script>
// @ is an alias to /src
import Hero from '@/components/Hero.vue'
import Package from '@/components/Package.vue'
import About from '@/components/About.vue'
import Why from '@/components/Why.vue'
import Contact from '@/components/Contact.vue'





export default {
  name: 'HomeView',
  components: {
    Hero,Package,About,Why,Contact
  },
    mounted(){
      window.scrollTo(0,0)
    }
}
</script>
