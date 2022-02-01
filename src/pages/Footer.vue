<template>
  <div>
    <footer class="col-md-10 m-auto mb-5 row">
      <!-- <div class="col-md-7 m-auto text-center">
        <i class="text-dark fab fa-instagram"></i>
        <i class="text-dark fab fa-facebook"></i>
        <i class="text-dark fab fa-whatsapp"></i>
      </div> -->

      <div class="col-md-4">
        <h1 style="font-size:1.6rem">Clothes Store</h1>
        <i class="text-dark fab fa-instagram"></i>
        <i class="text-dark fab fa-facebook"></i>
        <i class="text-dark fab fa-whatsapp"></i>
      </div>


      <div class="col-md-3">
        <p>Products</p>
        <p>Store</p>
        <p>Collection</p>

      </div>

      <div class="col-md-3">
        <p>Support</p>
        <p>Terms and conditions</p>
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
footer {
  border-radius: 0.25rem;
  border: none;
  box-shadow: 0 10px 20px 4px #e1e5e7;

  .fab {
    font-size: 2rem;
    padding-left: 0.4rem;margin-bottom:1rem;
    &:hover {opacity: 0.5;}
  }

  p{
    &:hover{color: #098697;border-left: solid 1px #1a1a1a;}
  }
}
</style>
