<template>
  <div class="home">
    <Article/>
    <Footer/>
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import Article from '../pages/Article.vue';
import Footer from '../pages/Footer.vue';

export default defineComponent({
  name: "Home",
  components:{Article, Footer}
})
</script>
