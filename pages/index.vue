<template>
  <div>
    <section class="hero">
      <div class="content hero-inner">
        <img class="hero-image" src="~/assets/hero.jpg">
        <div class="hero-overlay">
          <div class="hero-overlay-inner">
            <div class="hero-overlay-about">
            偶然のご縁がつながって、素敵な人生になったら素晴らしい。<br><br>
そんなことを目指しながら、読書会、ヨガ会、コーチング、コミュニティ作りをしています。<br><br>
自分自身が誰かのワクワクの象徴になれるように。
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="menu">
      <div class="content menu-inner">
        <a class="menu-item" href="#">
          <img class="menu-item-image" src="~/assets/profile.jpg">
          <div class="overlay">PROFILE</div>
        </a>
        <a class="menu-item" href="#">
          <img class="menu-item-image" src="~/assets/read.jpg">
          <div class="overlay">読書会</div>
        </a>
        <a class="menu-item" href="#">
          <img class="menu-item-image" src="~/assets/about.jpg">
          <div class="overlay">YOGA</div>
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
    border-radius: 20px;
  }

  &-overlay {
    position: absolute;
    padding: inherit;
    z-index: 1;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;

    &-inner {
      width: 100%;
      height: 100%;
      background: rgba(white, 0.4);
      display: flex;
      justify-content: center;
      align-items: center;
      border-radius: 20px;
    }

    &-about {
      width: 600px;
      text-align: center;
      font-size: 13pt;
      color: #333;
      word-break: break-all;
    }
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
      border-radius: 20px;
    }

    .overlay {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 20%;
      background: rgba(white, 0.7);
      display: flex;
      justify-content: center;
      align-items: center;
      letter-spacing: 0.2em;
      font-size: 15pt;
      border-radius: 0 0 20px 20px;
      opacity: 1;
      transition: all 0.3s;
    }
  }

  &-item:hover .overlay {
    opacity: 0.7;
  }
}

</style>
