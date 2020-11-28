<template>
  <div >
    <div class="container">
      <Navbar />
      <main>
        <div > 
          <nuxt />
        </div>
      </main>
    </div>
     <hr class="line">
     <div class="container">
      <Footer />
     </div>
  </div>
</template>
<script>
import Navbar from '@/components/Navbar';
import Footer from '@/components/Footer';

export default {
  components: {
    Navbar,
    Footer
  }
}
</script>
<style>

</style>
