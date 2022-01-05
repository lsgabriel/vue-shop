<template>
  <div class="home">
    <Header/>
    <Article/>
    <Footer/>
  </div>
</template>

<script>
import { defineComponent } from 'vue';
import Header from '../pages/Header.vue';
import Article from '../pages/Article.vue';
import Footer from '../pages/Footer.vue';

export default defineComponent({/* 
  name: "Home", */
  components:{Header, Article, Footer}
})
</script>
