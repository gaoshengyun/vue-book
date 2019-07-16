<template>
  <div class="home">
    <span class="text">012345</span><br>
    <span class="text">ABCDEF</span><br>
    <span class="icon-bookmark"></span>
    <span class="icon-clock"></span>
  </div>
</template>

<script>

export default {
  name: 'home',
 
}
</script>
<style lang="scss" scope>
  @import '../assets/styles/global.scss';
  .icon-bookmark{
    font-size: 30px;
    color: #f00;
  }
  .text{
    font-family: 'Days One';
    font-size: px2rem(30);
    color: orange;
  }
</style>


