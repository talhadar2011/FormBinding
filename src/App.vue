<template>
  <h1> Web Form</h1>
<<<<<<< HEAD
  <SignpForm/>
</template>

<script>
import SignpForm from './components/SignpForm.vue';
export default {
  name: 'App',
  components: {
    SignpForm
=======
  <SignUpForm/>
</template>

<script>
import SignUpForm from './components/SignpForm.vue'

export default {
  name: 'App',
  components: {
    SignUpForm
>>>>>>> DataBinding
  }
}
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
body{
  margin: 0px;
  background-color: #eee;
}
</style>
