<template>
  <div>
    <nav-header></nav-header>
    <router-view></router-view>
    <nav-footer></nav-footer>
  </div>
</template>

<script>
// @ is an alias to /src
import  axios  from  'axios'
export default {
  name:'nav-home',
  components: {

  },
  mounted() {
    let url = 'https://www.easy-mock.com/mock/5f670f277304034f4b754175/mall/a/haha#!method=get';
   axios.get(url).then(data => {
     console.log(data,'dfja')
   })
  }
}
</script>
