<template>
  <div id="app">
    <HelloWorld :data="data.groups"></HelloWorld>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import data from '../static/data'

export default {
  data(){
    return {
      data
    }
  },
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>

</style>
