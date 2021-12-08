<template>
  <img alt="Vue logo" src="./assets/count.jpg">
  <p>count: {{ $store.state.count }}</p>
  <!--點擊時增加觸發increment()-->
  <button @click="$store.commit('increment')">increment</button>
  <HelloWorld msg="Count The Number!"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
