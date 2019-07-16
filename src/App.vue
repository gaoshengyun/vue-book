<template>
  <div id="app">
    <div id="nav">
  
    </div>
    <router-view/>
  </div>
</template>
<script>
  import {mapGetters} from 'vuex'
  document.addEventListener('DOMContentLoaded',() => {
    const html = document.querySelector('html')
    let fontSize = window.innerWidth / 10
    fontSize = fontSize > 50 ? 50 : fontSize
    html.style.fontSize = fontSize + 'px'
  })
  export default {
    mounted() {
      this.$store.dispatch('setTest',156).then(()=>{
        console.log(this.test)
      })
    },
    computed: {
      ...mapGetters(['test'])
    },
  }
</script>
<style>

</style>
