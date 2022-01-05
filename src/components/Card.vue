<template>
    <div class="card">
      <router-link to="/details" style="text-decoration: none;">
            <img :src="require(`../assets/${imageUrl}`)" class="card-img-top" alt="..." />
            <div class="card-body">
              <h2 class="card-title">{{title}}</h2>
              <!-- <p class="card-text">
                This is a longer card with supporting text below as a natural
                lead-in to additional content. This content is a little bit
                longer.
              </p> -->
              <p class="price text-dark">{{priceProps}}</p>
              <a class="shop-icon text-dark" href="#">
                <i class="fas fa-shopping-bag position-relative">
                  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-primary">
                    +
                    <span class="visually-hidden">icon</span>
                  </span>
                </i>
              </a>
            </div>
            </router-link>
          </div>
</template>

<script>
import { defineComponent } from 'vue';
export default defineComponent({
    props:{
        imageUrl:{
            required:true
        },
        title:{
          required:true
        },
        priceProps:{
          required:true
        }
    }
})
</script>


<style lang="scss" scoped>
    .card { 
    border: none;box-shadow: 0 10px 20px 4px #e1e5e7;
    img{
        width: 19rem;height: 19rem;margin: auto;border-radius: 0.25rem;
    }
    p{font-weight: 300;color: #111111;}
    .price{font-size: 2rem;}
    .shop-icon{
      font-size: 2.2rem;float: right;padding-right: 1vw;
      
      &:hover{opacity: 0.7;}
        .badge{font-size: 0.7rem;
        
          &:hover{background-color: #1a1a1a;}
        }
    }
  }
</style>