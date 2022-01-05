<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light sticky-top">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">
          <img src="../assets/logo.svg" alt="" width="45" height="45" />
          <span style="color: #47b88c">Clothes Store</span>
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0"></ul>

          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link" href="#">Favorites</a>
            </li>

            <li
              class="nav-item"
              data-bs-toggle="modal"
              data-bs-target="#exampleModal"
            >
              <a href="#" class="nav-link">Categories</a>
            </li>

            <li class="nav-item">
              <button type="button" class="btn btn-dark position-relative">
                Cart
                <span
                  class="
                    position-absolute
                    top-0
                    start-100
                    translate-middle
                    p-2
                    bg-primary
                    border border-light
                    rounded-circle
                  "
                >
                  <span class="visually-hidden">New alerts</span>
                </span>
              </button>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Modal -->
    <div
      class="modal fade"
      id="exampleModal"
      tabindex="-1"
      aria-labelledby="exampleModalLabel"
      aria-hidden="true"
    >
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header">
            <h5 class="modal-title" id="exampleModalLabel">Modal title</h5>
            <button
              type="button"
              class="btn-close"
              data-bs-dismiss="modal"
              aria-label="Close"
            ></button>
          </div>
          <div class="modal-body m-auto">
            <button class="btn modal-btn text-primary">
              <i class="fas fa-shopping-bag" />
              <br />
              <p>Tops & T-Shirts</p>
            </button>

            <button class="btn modal-btn text-primary">
              <i class="fas fa-shopping-bag" />
              <br />
              <p>Jackets & Vests</p>
            </button>

            <button class="btn modal-btn text-primary">
              <i class="fas fa-shopping-bag" />
              <br />
              <p>Hoodies</p>
            </button>
          </div>
        </div>
      </div>
    </div>
</template>

<style lang="scss" scoped>
  .modal {
    .modal-btn {
      background-color: white;
      margin-left: 1rem;
      width: 8rem;
      height: 6rem;

      i {
        font-size: 1.8rem;
        color: #259e80;
      }
      p {
        font-size: 1rem;
        font-weight: 300;
        color: #2e2d2d;
      }

      &:hover {
        border: solid 2px #259e80;
      }
    }
}
</style>