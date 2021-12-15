<template>
  <div id="app">
    <Header/>
    <Main/>
    <Blog/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Blog from './components/Blog.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Blog,
    Footer
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+3&display=swap');
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 20px;
}
.btn{
  background-color: #38b6a1;
  color: white;
}
.verde{
  color: #38b6a1;
}
.font{
  font-family: 'Playfair Display', serif;
}
.title{
  font-family: 'Roboto', sans-serif;
}
</style>
