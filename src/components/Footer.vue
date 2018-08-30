<template>
      <footer class="footer">Brook+Lynn &copy; {{date}}</footer>
</template>

<script>
    export default {
        name: 'Footer',
        data() {
            return {
                date: new Date().getFullYear()
            }
        }
    }    
</script>
