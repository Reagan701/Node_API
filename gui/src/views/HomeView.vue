<template>
  <div class="home">
    <h2>This is the Home page</h2>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>
.home {
  background-image: url(https://i.postimg.cc/mZwkKwtG/pick.png);
  background-size: cover;
  background-position:center;
  background-repeat: no-repeat;
  height:100vh;
  color: white;
}
</style>
