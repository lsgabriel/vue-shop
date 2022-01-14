<template>
    <div class="main-container col-md-10 m-auto mb-4">
        <div class="row">
            <div class="col-md-4">
                <img src="../assets/pic1.jpeg" class="product-img"/> 
            </div>
            <div class="col-md-7 product-desc">
                <h1>Nike X</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse pharetra est id arcu varius, ac fermentum lectus varius. Pellentesque maximus eu dolor id faucibus. Maecenas mi est, molestie eget posuere non, pharetra convallis nibh.</p>
                <p class="price">210.00</p>
            </div>
        </div>
    </div>
    <Footer/>
</template>

<script>
import { defineComponent } from 'vue';
import Footer from './Footer.vue';

export default defineComponent({
  components:{Footer}
})
</script>

<style lang="scss" scoped>
@mixin customBorder() {border-radius: 0.25rem;}

    .main-container{

        .product-img{
            width: 100%;min-height: 63vh;object-fit: cover;
            @include customBorder();
        }

        .product-desc{
            p{color: #1a1a1a;font-size: 1.5rem;}
            p.price{color: #47B88C;font-size: 2rem;}
        }
    }
</style>