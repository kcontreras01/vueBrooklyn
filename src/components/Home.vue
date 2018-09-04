<template>
  <div class="hello">
    <title>Brook+Lyn</title>
    <div>
      <h1>Brook+Lyn</h1>
      <img :src="logo" :key="logo" id="bigimage">
    </div>

    <div id="clothing-container">
        <img v-for="shirt in clothing" :src="shirt.src" alt="shirt" class="clothing">
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

      clothing: [
        {
           src: require('../assets/shirt-1.jpg') 
        },
        {
           src: require('../assets/shirt-2.jpg') 
        },
        {
           src: require('../assets/shirt-3.jpg') 
        },
      ]
    }
  }
}
</script>