<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container">
      <a class="navbar-brand col-6 col-md-2" href="#">Sticker<span class="orange">z.</span></a>
      <button class="navbar-toggler" type="button" @click="openMenu" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarTogglerDemo02" :class="{ show: this.open}">
        <ul class="navbar-nav mb-2 mx-auto mb-lg-0 col-12 col-md-8 d-flex justify-content-around">
          <li class="nav-item">
            <a href="#">Products</a>
          </li>
          <li class="nav-item">
            <a href="#">Features</a>
          </li>
          <li class="nav-item">
            <a href="#">Accessories</a>
          </li>
          <li class="nav-item">
            <a href="#">Delivery</a>
          </li>
          <li class="nav-item">
            <a href="#">Contact</a>
          </li>
        </ul>
        <form class="d-flex col-12 col-md-3">
          <input class="form-control" type="search" placeholder="Search" aria-label="Search">
          <button class="btn" type="submit"><fa icon="search" /></button>
        </form>
      </div>
    </div>
  </nav>
</template>


<script>
export default {
  data() {
    return {
      open: false
    };
  },
  methods: {
    openMenu() {
      this.open = !this.open;
    }
  },
};

</script>