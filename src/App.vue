<template>
  <!-- <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view /> -->
  <Header/>
</template>

<script>
import { defineComponent } from 'vue';
import Header from "./pages/Header.vue";

export default defineComponent({
  components:{Header}
})
</script>

