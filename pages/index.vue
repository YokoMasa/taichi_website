<template>
  <div>
    <section class="hero">
      <div class="content hero-inner">
        <img class="hero-image" src="~/assets/placeholder.jpg">
        <a class="hero-nav" href="#">
          <div class="hero-nav-inner">読書会はこちら</div>
        </a>
      </div>
    </section>

    <section class="menu">
      <div class="content menu-inner">
        <a class="menu-item" href="#">
          <img class="menu-item-image" src="~/assets/placeholder.jpg">
          <div class="overlay">ABOUT</div>
        </a>
        <a class="menu-item" href="#">
          <img class="menu-item-image" src="~/assets/placeholder.jpg">
          <div class="overlay">PROFILE</div>
        </a>
        <a class="menu-item" href="#">
          <img class="menu-item-image" src="~/assets/placeholder.jpg">
          <div class="overlay">読書会</div>
        </a>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  components: {
    
  }
}
</script>

<style scoped lang="scss">
.hero {
  height: 600px;

  &-inner {
    position: relative;
  }

  &-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 30px;
  }

  &-nav {
    position: absolute;
    bottom: 50px;
    left: 50px;
    display: inline-block;
    width: 300px;
    height: 50px;
    background: rgba($color: white, $alpha: 0.5);
    border-radius: 30px;
    transition: background 0.2s;

    &-inner {
      width: 100%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      font-size: 10pt;
      font-weight: 600;
    }
  }

  &-nav:hover {
    background: rgba($color: white, $alpha: 0.7);
  }
}

.menu {
  height: 400px;

  &-inner {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &-item {
    position: relative;
    width: 30%;
    height: 70%;
    
    &-image {
      width: 100%;
      height: 100%;
      object-fit: cover;
      border-radius: 30px;
    }

    .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba($color: black, $alpha: 0.3);
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      font-size: 19pt;
      font-weight: 500;
      border-radius: 30px;
      opacity: 0;
      transition: all 0.3s;
    }
  }

  &-item:hover .overlay {
    opacity: 1;
  }
}

</style>
