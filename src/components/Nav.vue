<template>
	<div> 
        <nav> 
   			<router-link class="spacing" v-for="routes in links" :key="routes.id" :to="`${routes.page}`">{{routes.text}}</router-link>
   		</nav> 
	</div>
</template>

<script>
    export default {
        data() {
            return {
                links: [
                {
                  id: 0,
                  text: 'Home',
                  page:'/'
                },
                {
                  id: 1,
                  text: 'About',
                  page:'/About'
                },
                {
                  id: 2,
                  text: 'Shop',
                  page:'/Shop'
                },
                {
                  id: 3,
                  text: 'Contact',
                  page:'/Contact'
                }
                ]
            }
        }
    }
</script>

<style> 
  .spacing { 
    Margin-right: 10px; 
  } 
</style>