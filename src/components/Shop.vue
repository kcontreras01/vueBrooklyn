<template>
    <div id="items-container">
        <stack :column-min-width="300" :gutter-width="15" :gutter-height="15" monitor-images-loaded>
            <stack-item v-for="(item, i) in items" :key="i" style="transition: left 300ms, top 300ms" :class="'stack'">
                <img :src="item.src" :class="'shop-images'">
            </stack-item>
        </stack>
</waterfall>

    </div>
</template>

<script>
    import {Stack, StackItem} from 'vue-stack-grid'

    export default {
        name: 'Shop',
        components: {Stack, StackItem},
        data() {
            return {
                items: [
                {
                    name: '',
                    price: '',
                    src: require('../assets/earrings.jpg')
                },
                {
                    name: '',
                    price: '',
                    src: require('../assets/necklaces.jpg')
                },
                {
                    name: '',
                    price: '',
                    src: require('../assets/pendant.jpg'),
                },
                {
                    name: '',
                    price: '',
                    src: require('../assets/tiara.jpg'),
                },
                {
                    name: '',
                    price: '',
                    src: require('../assets/heart.jpg'),
                },
                {
                    name: '',
                    price: '',
                    src: require('../assets/ring.jpg'),
                },
                {
                    name: '',
                    price: '',
                    src: require('../assets/crystal.jpg'),
                },
                {
                    name: '',
                    price: '',
                    src: require('../assets/key.jpg'),
                },
                {
                    name: '',
                    price: '',
                    src: require('../assets/dreamcatcher.jpg'),
                },
                ]
            }
        }
    }
</script>

<style scoped>
    .shop-images {
        border: none;
        width: 80%;
        /*height: 100%;*/
    }

    #items-container {
        width: 60%;
        margin: auto;
    }
</style>