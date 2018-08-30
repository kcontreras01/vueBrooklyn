<template>
  <div class="hello">
    <title>Brook+Lyn</title>
    <div>
      <h1>Brook+Lyn</h1>
      <img :src="logo" :key="logo" id="bigimage">
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      show: false,
      logo: require('../assets/home-rings.png'),
    }
  }
}
</script>