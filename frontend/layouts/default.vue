<template>
<div>
  <div class="flex justify-center" >
    <NavBar />
  </div>
  <section class="hero">
        <div class="hero-inner">
        </div>
  </section>
  <div class="flex justify-center" >
   <div class="max-w-screen-lg flex flex-col min-h-screen w-full">
    <Buttons />
    <Nuxt class="flex-grow" />
    <Footer />
   </div>
  </div>
  <div hidden id="snipcart" data-api-key="ODhhNWUxOGEtNTk0OC00OTQwLWJkOWMtM2M1ZmNjODU1ZDJhNjM3MzMyNzM0NjM1OTMyNjcz"></div>
</div>
</template>

<script>
import NavBar from './../components/Navbar'
import Footer from './../components/Footer'
import Buttons from './../components/Buttons'

export default {
  scrollToTop: false,
  components: {
    NavBar,
    Footer,
    Buttons
  }
}
</script>


<style scoped>
.hero {
    /* Sizing */
    width: 100vw;
    height: 90vh;
    
    /* Flexbox stuff */
    display: flex;
    justify-content: center;
    align-items: center;
    
    /* Text styles */
    text-align: center;
    color: white;
    
    /* Background styles */
    background-image: linear-gradient(rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.5)), url(@/assets/hero.png);
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    background-attachment: fixed;
}
</style>