<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import  axios  from  'axios'
export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  mounted() {
    let url = 'http://www.easy-mock.com/mock/5f670f277304034f4b754175/mall/a/haha#!method=get';
   axios.get(url).then(data => {
     console.log(data)
   })
  }
}
</script>
