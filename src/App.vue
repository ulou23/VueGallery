<template>
  <div id="app">
    <transition name="fade" mode="out-in">

      <router-view></router-view>
    </transition>
  </div>
</template>

<script>

export default {
  name: 'app',
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
  .fade-enter-active, .fade-leave-action{
    transition: opacity .5s ease-out;
  }
  .fade-enter, .fade-leave-to {
    opacity: 0;
  }
</style>
