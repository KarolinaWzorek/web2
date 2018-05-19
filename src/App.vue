<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>bfgfg   Witaj w systemie zapisow do czegos tam  {{email.toLowerCase()}}</h1>

<div v-if="!klikniete">   
<input type="email" v-model="email">
<button @click="LogIn()">zalog</button>
  </div>

  <div v-else>  zalogowany jako {{email}}
    <a href @click="LogOut()">wyloguj </a>
    </div>
        </div>

</template>







<script>
import "milligram";

export default {
  name: 'app',
  data () {
    return {
      email: 'dgfgd', 
      klikniete: false
    }
  }


,
methods: {
  LogIn() {
  this.klikniete=true;
},

LogOut() {
  this.klikniete=false;

}

}
}
</script>



