<template>
  <div>
    <Navbar/>
    <Details/>
    <Footer/>
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import Navbar from '../pages/Navbar.vue';
import Details from '../pages/Details.vue';
import Footer from '../pages/Footer.vue';

export default defineComponent({
  components:{Navbar, Details, Footer}
})
</script>
