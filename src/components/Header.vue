<script setup>

</script>

<template>
  <nav>
    <router-link class="text-white p-2 mx-4 hover:text-green-500" to="/" >Home</router-link>
    <router-link class="text-white p-2 mx-4 hover:text-green-500" to="/about" >About</router-link>
  </nav>
</template>



<style scoped>
  nav{
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    width: 100%;
    padding: 20px;
    background: rgba( 26, 26, 26, 0.4 );
    backdrop-filter: blur( 7px );
    -webkit-backdrop-filter: blur( 7px );
    border-bottom: 1px solid rgba( 255, 255, 255, 0.18 );
  }

</style>
