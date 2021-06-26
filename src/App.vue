<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3.0 + Vite" />
  <ApiTest msg="mex"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import ApiTest from './components/ApiTest.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    ApiTest
  }
}
</script>
