<template>
  <div class="hello">
    <title>Brook+Lyn</title>

    <div class="main">
      <h1>Brook+Lyn</h1>

      <img :src="logo" :key="logo" id="bigimage">

      <p>Brook+Lynn &copy; {{date}}</p>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      show: false,
      date: new Date().getFullYear(),
      logo: require('../assets/home-rings.png'),
    }
  }
}
</script>