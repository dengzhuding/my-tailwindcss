<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="app-div">
    <h1 class="text-amber-400 text-xl">hello world</h1>
    <h2 class="app-color-red">this is use scss global variable $red</h2>
    <h2 class="app-color-blue">this is use scss local variable $blue</h2>
    <h2 class="app-color-yellow">this is import external scss style for $yellow</h2>
  </div>
</template>

<style scoped lang="scss">
@import url(@style/app-pieces.scss);
$blue: rgb(113, 113, 224);
.app-div {
  .app-color-red {
    color: $red;
  }
  line-height: 2rem;
}
.app-color-blue {
  color: $blue;
}
</style>
