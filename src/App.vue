<template>
  <LoginBox/>
</template>

<script>
import LoginBox from './components/LoginBox.vue'

export default {
  name: 'App',
  components: {
    LoginBox,
  }
}
</script>

<style>
body {
  background-image: url('./assets/background.png');
  background-size: 100%;
}

</style>
