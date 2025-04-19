<script setup>
 const weater = 'r' // s, pc, r, c, ci
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
</template>

<style scoped>
 
</style>
