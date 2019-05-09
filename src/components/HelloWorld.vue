<template>
  <ul>
    <li v-for="(item,index) in data" :key="index">
      {{item.name}}
      <HelloWorld v-if="item.child" :data="item.child"></HelloWorld>
      <HelloWorld v-if="item.groups" :data="item.groups"></HelloWorld>
    </li>
  </ul>
</template>

<script>
import datas from '../../static/data'
import HelloWorld from './HelloWorld'
export default {
  name:'HelloWorld',
  data(){
    return {
      datas
    }
  },
  components:{
    HelloWorld
  },
  created() {

  },
  props:['data'],
  mounted() {
    // console.log(datas)
  }
}
</script>
<style scoped  lang="">

</style>