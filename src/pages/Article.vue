<template>
    <div class="products-grid m-3 col-md-9 m-auto">
      <div class="mt-2 mb-5 row row-cols-1 row-cols-md-3 g-5">
        <div class="col">
          <Card imageUrl="pic1.jpeg" title="Nike X" priceProps="210.00" />
        </div>
        <div class="col">
          <Card imageUrl="pic3.jpeg" title="Nike Vapor" priceProps="250.00" />
        </div>
        <div class="col">
          <Card imageUrl="pic1.jpeg" title="Nike X" priceProps="200.00" />
        </div>
        <div class="col">
          <Card imageUrl="pic1.jpeg" title="Nike Two" priceProps="200.00" />
        </div>
        <div class="col">
          <Card imageUrl="pic3.jpeg" title="Nike Y" priceProps="250.00" />
        </div>
        <div class="col">
          <Card imageUrl="pic3.jpeg" title="Nike One" priceProps="190.00" />
        </div>
      </div>
    </div>

    <div class="section col-md-10 m-auto mb-5">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed scelerisque
        est pulvinar ex porttitor dignissim. Phasellus hendrerit, nisi diam
        pretium lectus
      </p>
    </div>
</template>

<script>
import { defineComponent } from "vue";
import Card from '../components/Card.vue';

export default defineComponent({
  components: { Card },
});
</script>

<style lang="scss" scoped>
.products-grid {
  .card {
    border: none;
    box-shadow: 0 10px 20px 4px #e1e5e7;

    img {
      width: 19rem;
      margin: auto;
      border-radius: 0.25rem;
    }
    p {
      font-weight: 300;
      color: #111111;
    }
    .price {
      font-size: 2rem;
      color: #259e80;
    }

    .shop-icon {
      font-size: 2.2rem;
      color: #098697;
      float: right;
      padding-right: 1vw;

      &:hover {
        opacity: 0.7;
      }

      .badge {
        font-size: 0.7rem;
        background-color: #47b88c;

        &:hover {
          background-color: #1a1a1a;
        }
      }
    }
  }
}

.section {
  background-image: linear-gradient(to bottom right, #47b88c, #259e80);
  height: 35vh;
  color: whitesmoke;
  padding: 15px;
  font-size: 2rem;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 0.25rem;
  font-weight: 300;
}
</style>