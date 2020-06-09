<template>
  <div>
    <main-header></main-header>
    <nuxt style="margin-top: 80px;"/>
    <main-footer></main-footer>
  </div>
</template>
<script>
import MainHeader from '~/components/MainHeader'
import MainFooter from '~/components/MainFooter'

export default {
  components: {
    MainHeader, MainFooter
  }
}
</script>
<style>
html {
  font-family: 'Noto Sans JP', sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  color: #555;
}
a { text-decoration: none;}
a:link { color: #555; }
a:visited { color: #555; }
a:hover { color: #555; }
a:active { color: #555; }

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.content {
  max-width: 1100px;
  height: 100%;
  margin-left: auto;
  margin-right: auto;
  padding: 20px;
}
</style>
