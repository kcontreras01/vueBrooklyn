<template>
  <div id="app"  class="main">
    <Nav></Nav>
    <router-view/>
    <Footer></Footer>
  </div>
</template>

<script>
  import Nav from './components/Nav'
  import Footer from './components/Footer'

export default {
  name: 'App',
  components: {Nav, Footer}
}
</script>

<style src="./style.css"></style>
