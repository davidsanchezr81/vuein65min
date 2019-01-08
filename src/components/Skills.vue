<template>
  <div class="hello">
    {{ name}} 

    {{ btnState ? 'The Button is Disabled' : 'The button is Enabled'}}



    <!-- Continue on min 21:00 https://www.youtube.com/watch?v=78tNYZUS-ps -->

    <button v-on:click="changename" v-bind:disabled = "btnState">Change Name</button>
  </div>
</template>

<script>
export default {
  name: 'Skills',
  data(){

    return {
      name : 'David',
      btnState:false
    }
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
