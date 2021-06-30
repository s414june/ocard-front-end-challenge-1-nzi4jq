<template>
  <div id="app">
    <img alt="Vue logo" src="https://vuejs.org/images/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  metaInfo:{
    meta:[
      {
        property:"tracker:google-analytics",
        content:"UA-XXXXX-Y"
      },
      {
        property:"tracker:google-tag-manager",
        content:"GTM-XXXX"
      },
      {
        property:"tracker:facebook-pixel",
        content:"123456789010"
      }
    ]
    
  }
}

</script>
<script>
  gtag('config', 'UA-12345678-1');
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
