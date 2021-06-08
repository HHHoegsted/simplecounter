<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <Counter />
    <CounterSquared />
    <Buttons />
    <ColorCode />
  </div>
</template>

<script>


export default {
  name: 'Home',
  components: {
    'Counter' : require('@/components/Counter.vue').default,
    'CounterSquared' : require('@/components/CounterSquared.vue').default,
    'Buttons' : require('@/components/Buttons.vue').default,
    'ColorCode' : require('@/components/ColorCode.vue').default
  }
}
</script>

<style scoped>
div{
  margin-bottom: 10px;
}
.counter{
  font-size: 80px;
}
</style>