<template>
    <button class="btn btn-dark">{{title}}</button>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  components:{},

   props:{
        title:{
            required:true
        },
    }
})
</script>

<style lang="scss" scoped>
    button{
        margin:4px;

        &:hover{
            background-color: #47B88C;border:none;
        }

        @media(max-width: 480px) {
                width: 100%;margin:0;font-size:1.6rem;margin-bottom:1.1rem;
            }
    }
</style>