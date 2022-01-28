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
    }
</style>