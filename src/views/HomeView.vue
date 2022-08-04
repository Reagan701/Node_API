<template>
  <div class="home">
    <img id="logo" src="https://i.postimg.cc/TYm7hHJ4/pick-removebg-preview.png" alt="">
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
  background-image: url(https://i.postimg.cc/LXtKt6zr/pasta-5120x2880-tomato-olives-garlic-olive-5k-16053.jpg);
  background-size: cover;
  background-position:center;
  background-repeat: no-repeat;
  height:100vh;
  color: white;
}
#logo{
  height:100%;
  width:70%;
  padding: 0 0 100px 0;
}
</style>
