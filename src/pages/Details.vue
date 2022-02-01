<template>
<div class="top"></div>
    <div class="main-container col-md-10 m-auto mt-5">
        <div class="row">
            <div class="col-md-4">
                <img src="../assets/pic1.jpeg" class="product-img"/> 
            </div>
            <div class="col-md-7 product-desc">
                <h1>Nike X</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse pharetra est id arcu varius, ac fermentum lectus varius. Pellentesque maximus eu dolor id faucibus. Maecenas mi est, molestie eget posuere non, pharetra convallis nibh.</p>
                <p class="price">210.00</p>

                <Button title="Add to Cart"/>
                <Button title="Favorite"/>
            </div>
        </div>
    </div>

    <div class="bottom mb-5"></div>
    <Footer/>
</template>

<script>
import { defineComponent } from 'vue';
import Footer from './Footer.vue';
import Button from '../components/Button.vue';

export default defineComponent({
  components:{Button,Footer}
})
</script>

<style lang="scss" scoped>
@mixin customBorder() {border-radius: 0.28rem;}

    .main-container{

        .product-img{
            width: 100%;height: 62vh;object-fit: cover;
            @include customBorder();

            @media(max-width: 499px) {
                height: 48vh;padding:10px;
            }
        }

        .product-desc{
            p{color: #1a1a1a;font-size: 1.5rem;}
            p.price{color: #47B88C;font-size: 2.3rem;}
        }   
    }

    .bottom{
        background-color: #47B88C;width:84%;height:0.25rem;margin:auto;margin-top: 18vh;
    } 
    .top{
        background-color: #47B88C;width:84%;height:0.25rem;margin:auto;
    } 
</style>