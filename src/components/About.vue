<template>
  <div>
    <h2>About</h2>
      
      <p>In late 2008, Mimi Jung started a blog, documenting her unique personal style. After being named one of New York's top ten fashion bloggers by Huffington Post, Mimi launched a self-designed jewelry collection titled "Surrounded."</p>
      
      <p>Her debut collection was featured by Lucky Magazine, Refinery 29 and New York Magazine and carried by boutiques across the country, including ShopBop and Anthropologie. Her most recent collection, titled "Medaled", is set to launch this fall.</p>

    <h2>Press</h2>
      
      <a v-for="info in press" :href="info.link"><img :src="info.src"></a>
  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
          press: [
            {
              link: 'http://www.nbc.com',
              src: require('../assets/press-nbcnewyork.gif') 
            },
            {
              link: 'http://www.huffingtonpost.com',
              src: require('../assets/press-huffpost.gif') 
            },
            {
              link: 'http://www.luckymag.com',
              src: require('../assets/press-logo_lucky.gif') 
            },
            {
              link: 'http://www.marieclaire.com',
              src: require('../assets/press-marieclaire.gif') 
            },
          ]
        }
    }
}
</script>