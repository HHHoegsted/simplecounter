<template>
    <div>
      <input v-model="colorCode" type="text" placeholder="Enter Color Code">
    </div>
</template>

<script>
export default {
  computed: {
    colorCode:{
      get(){
        return this.$store.state.colorCode;
      },
      set(colorValue){
        this.$store.dispatch('changeColorCode', colorValue);
      }
    }
  },
}
</script>

<style>

</style>