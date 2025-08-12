<template>
  <form>
    <label>Email:</label>
<<<<<<< HEAD
    <input type="email" placeholder="Enter you E-Mail Address">
  </form>
=======
    <input type="email" v-model="email" placeholder="Enter you E-Mail Address">
    
    <label>Password:</label>
    <input type="password" v-model="password" placeholder="Enter you Password">
  </form>
  <p>
    Email:{{ email }}
    Password:{{ password }}
  </p>
>>>>>>> DataBinding
</template>

<script>
export default {
<<<<<<< HEAD

=======
    data(){
        return{
            email:'',
            password:''

        }
    }
>>>>>>> DataBinding
}
</script>

<style>
    form{
        max-width: 420px;
        margin: 30px auto;
        background: rgb(252, 250, 250);
        text-align: left;
        padding: 40px;
        border-radius: 10px;
    }
    label{
        color: #aaa;
        display: inline-block;
        margin:25px 0 15px;
        font-size:0.6em;
        text-transform: uppercase;
        letter-spacing: 1px;
        font-weight: bold;
    }
    input{
        display: block;
        padding: 10px 6px;
        width: 100%;
        box-sizing: border-box;
        border: none;
        border-bottom:1px solid #ddd ;
        border-radius: 5px;
        color:#555;
    }
</style>