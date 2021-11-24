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
  font-family: Helvetica, Arial, sans-serif;
  height: 100vh;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


.centratura {
  width: 80%;
  margin: 0 auto;
}

</style>
