<template>
  <div class="header">
      <div class="header-inner">

          <div class="header-logo">
              <span class="header-logo-text">Taichi Shibuki</span>
          </div>

          <div class="header-menuWrapper">
              <a href="#" class="header-menu">YOGA</a>
              <a href="#" class="header-menu">読書会</a>
              <nuxt-link to="/profile" class="header-menu">PROFILE</nuxt-link>
          </div>

      </div>
  </div>
</template>
<script>
export default {

}
</script>
<style scoped lang="scss">
.header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 80px;
    background: white;
    z-index: 5;

    &-inner {
        max-width: 1100px;
        height: 100%;
        margin-left: auto;
        margin-right: auto;
        position: relative;
    }

    &-logo {
        position: absolute;
        width: 300px;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;

        &-text {
            font-size: 20pt;
            font-weight: 700;
        }
    }

    &-menuWrapper {
        position: absolute;
        right: 0;
        max-width: 700px;
        height: 100%;
        display: flex;
        flex-direction: row-reverse;
        align-items: center;
    }

    &-menu {
        margin: 0 30px;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        text-decoration: none;
        font-size: 12pt;
        font-weight: 600;
        transition: color 0.2s;
    }

    &-menu:hover {
        color: #777;
    }
}
</style>