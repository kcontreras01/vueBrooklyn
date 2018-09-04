<template>
	<div id="nav"> 
        <nav> 
   			<router-link class="spacing" v-for="routes in links" :key="routes.id" :to="`${routes.page}`">{{routes.text}}</router-link>

            
   		</nav> 
            <div id="icons">
                <font-awesome-icon icon="search"/>
                <font-awesome-icon icon="shopping-cart"/>
            </div>
        
	</div>
</template>

<script>
    import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

    export default {
        components: {FontAwesomeIcon},
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