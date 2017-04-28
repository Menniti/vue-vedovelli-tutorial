
<script>

  import CcUsers from './components/users/main.vue'

  export default {
    
    name:'Codecasts-App',

    components: {
      CcUsers
    },

    computed:{
      user() {
        const { name, email } = this.$store.state.user
        return `O usuário é 
          ${name} e possui o email
          ${email}`
        
      }
    }
  }
</script>



<template>
  
  <div>
    <h1>Welcome Vue2</h1>

    <h4> {{user}} </h4>

    <hr>

    <cc-users></cc-users>

  </div>

</template>