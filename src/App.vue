<template>
  <div id="app">
    <!-- nav bar -->
    <header>
      <Header/>
    </header>
    <main>
      <!-- pagina principale -->
      <MainBody/>
    </main>
    <!-- footer -->
    <footer>
      <FootPage/>
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import MainBody from './components/mainBody.vue';
import FootPage from './components/footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    MainBody,
    FootPage,
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}


</style>
