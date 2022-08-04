<template>
  <div id="main">
    <Cards />
  </div>
</template>

<script>
import Cards from "../components/Cards.vue";
export default {
  components: {
    Cards,
  },
};
</script>

<style>

#main{
  background-image: url(https://i.postimg.cc/LXtKt6zr/pasta-5120x2880-tomato-olives-garlic-olive-5k-16053.jpg);
  background-size: cover;
  background-position:center;
  background-repeat: no-repeat;
  height:100%;
  color: white;
}

#registerzone{
  padding: 50px 0 0 0;
}

#cardzone{
  padding: 40px 50px 40px 50px;
  border-radius: 20px;
}

.card, .btn, input{
  border-radius:0 ;
}
</style>