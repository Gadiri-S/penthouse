<template>
  <div class="home">

    <HeroFr/>
    <WhyFr/>
        <PackageFr/>
        <AboutFr/>
        <ContactFr/>


  </div>
</template>

<script>
// @ is an alias to /src

import HeroFr from '@/components/Hero-fr.vue'
import PackageFr from '@/components/Package-fr.vue'
import AboutFr from '@/components/About-fr.vue'
import WhyFr from '@/components/Why-fr.vue'
import ContactFr from '@/components/Contact-fr.vue'





export default {
  name: 'HomeView',
  components: {
    HeroFr,PackageFr,AboutFr,WhyFr,ContactFr
  },
    mounted(){
      window.scrollTo(0,0)
    }
}
</script>
