<template>
  <div id="app">
    <Pokemon />
  </div>
</template>

<script>
import { shallowMount } from '@vue/test-utils'
import Pokemon from './components/Pokemon.vue'

// helper function that mounts and returns the rendered component
function getMountedComponent(Component, propsData) {
  return shallowMount(Component, {
    propsData
  })
}

export default {
  components: {
    Pokemon
  }
}
</script>

<style lang="scss">
  @import url('https://use.fontawesome.com/releases/v5.8.2/css/all.css');

  body {
    margin: 0;
    padding: 0;
  }
</style>