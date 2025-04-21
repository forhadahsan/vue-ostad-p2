<script setup>
 const weater = 'r' // s, pc, r, c, ci

 const weekends = false // true, false
</script>

<template>
  <div>
    <h2>Hello Vue</h2>
    <p v-if="weater=='s'">Sunny</p>
    <p v-else-if="weater=='pc'">partials cloud</p>
    <p v-else-if="weater=='r'">Rain</p>
    <p v-else-if="weater=='c'">cloud</p>
    <p v-else-if="weater=='ci'">cyclone</p>
  </div>
  <div>
    <h2>Weather Loop (v-if & v-else-if)</h2>
    <p v-if="weater=='s'">Sunny</p>
    <p v-else-if="weater=='pc'">Partially Cloudy</p>
    <p v-else-if="weater=='r'">Rain</p>
    <p v-else-if="weater=='c'">Cloudy</p>
    <p v-else-if="weater=='ci'">Cyclone</p>
  </div>
  <div>
    <h2>Weather Loop (v-Show)</h2>
    <p v-show="weater=='s'">Sunny</p>
    <p v-show="weater=='pc'">Partially Cloudy</p>
    <p v-show="weater=='r'">Rain</p>
    <p v-show="weater=='c'">Cloudy</p>
    <p v-show="weater=='ci'">Cyclone</p>
  </div>
  <div>
    <h2>Weekend </h2>
    <p class="h-10 flex items-center justify-center" :class="weekends?'bg-red-500 text-4xl':'bg-green-400 text-2xl'">Weekend</p>
  </div> 
</template>

<style scoped>
 
</style>
