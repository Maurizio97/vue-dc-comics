<template>
  <div id="app">
    <!-- header -->
    <Header/>

    <!-- main -->
    <main>
      <Section/>

    </main>

    <!-- footer -->
    <Footer/>
    
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Section from './components/Section.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Section,
    Footer
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}


</style>
