<template>
  <form>
    <label>Email:</label>
<<<<<<< HEAD
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
=======
    <input type="email" v-model="email" placeholder="Enter your E-Mail Address">
    
    <label>Password:</label>
    <input type="password" v-model="password" placeholder="Enter your Password">

    

    <label>Role:</label>
    <select v-model="role">
        <option value="developer">Developer</option>
        <option value="devops">DevOps</option>
        <option value="Manager">Manager</option>
        <option value="teamlead">TeamLead</option>
    </select>

    <label>Skills:</label>
    <input type="text" v-model="tempSkill" @keyup="addSkill" placeholder="Enter your Skills">
    <div v-for="skill in Skills" :key="skill" class="pill">
      <span  @click="deleteSkill(skill)">  {{ skill }}</span>
    </div>

    <div class="terms">
        <input type="checkbox" v-model="terms" required>
        <label>Accept Terms and Conditions</label>

    </div>
    <div class="submit">
            <button>Create Account</button>
    </div>
</form>

>>>>>>> KeybordEvent
</template>

<script>
export default {
<<<<<<< HEAD

=======
    data(){
        return{
            email:'',
            password:'',
            role:'developer',
            terms:false,
            tempSkill:'',
            Skills:[]

        }
    },
    methods:{
        addSkill(e) {
            if(e.key==="Enter" && this.tempSkill){
                if(!this.Skills.includes(this.tempSkill))
                {
                    this.Skills.push(this.tempSkill)
                }
                this.tempSkill=''

            }
        },
        deleteSkill(skill){
            this.Skills=this.Skills.filter((item)=>item!==skill)
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
    input,select{
        display: block;
        padding: 10px 6px;
        width: 100%;
        box-sizing: border-box;
        border: none;
        border-bottom:1px solid #ddd ;
        border-radius: 5px;
        color:#555;
    }
    input[type="checkbox"]{
        display: inline-block;
        width: 16px;
        margin: 0 10px 0 0;
        position: relative;
        top: 2px;
    }
    .pill{
        margin: 10px;
        display: inline-block;
        background:#eee ;
        border-radius: 20px;
        padding: 6px 12px;
        cursor: pointer;
        letter-spacing: 1px;
        font-weight: bold;
        font-size: 12px; 
    }
    button{
        background: #eee;
        padding: 10px 20px;
        border:none;
        border-radius: 25px;
        font-size: 16px;
        font-weight: bold;
        color:#555;
        letter-spacing: 1px;
        margin:20px
    }
    .submit{
                text-align: center;

    }
</style>