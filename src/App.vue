<template>
  <h1> Web Form</h1>
  <SignpForm/>
</template>

<script>
import SignpForm from './components/SignpForm.vue';
export default {
  name: 'App',
  components: {
    SignpForm
  }
}
</script>

<style>
#app {
 margin: 0;
 text-align: center;
}
</style>
