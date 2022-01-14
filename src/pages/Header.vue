<template>
    <header >
        <div class="content">
            <h1>Clothes Store </h1>
            <p style="font-weight:300;padding-left:0.4rem">buy something new.</p>
        </div>
    </header>
    <Navbar/>
</template>

<script>
import { defineComponent } from "vue";
import Navbar from "./Navbar.vue";
export default defineComponent({
    components:{Navbar}
})
</script>


<style lang="scss" scoped>
    header{
        height: 100vh;background-image: url("../assets/wave.svg");
        background-size:contain;background-repeat: no-repeat;background-position: bottom;
        display: flex;align-items: center;justify-content: center;background-attachment: fixed;
        .content{line-height: 0.1rem;}
    }
    
</style>