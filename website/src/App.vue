<template>
  <div id="app">
    <div id="logo">
      <img id="fire-logo" alt="Fire logo" src="./assets/fire.png">
    </div>
    <div id="title">
      <h1>Vacuate</h1>
    </div>
    <Services msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import Services from './components/Services.vue'

export default {
  name: 'App',
  components: {
    Services
  }
}
</script>

<style>

/*Main fire logo styling*/
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 1%;
  display: flex;
}

/* Fire Logo size */
#fire-logo{
  width: 16%;
  height: 90%;
}

#logo{
  margin-top: 3%;
  margin-right: 0;
  margin-left: 20%;
  padding: 0;
  font-family:  Arial, Helvetica, sans-serif;
  color: #bb86fc;
}

#title{
  margin-top: 3%;
  margin-left: 0;
  font-family:  Arial, Helvetica, sans-serif;
  color: #bb86fc;
}

/* Set overall bg to shade of grey*/
body{
  background: #262a2e;
}
</style>
