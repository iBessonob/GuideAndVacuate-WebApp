<template>
  <div class="intro">
    
  </div>
</template>

<script>

//firebase setup
import * as firebase from 'firebase';

console.log("Testing for debugging purposes");
let app = firebase.initializeApp({
  databaseURL: 'https://hackmit-df9ea.firebaseio.com/'
});
let dbRef = app.database().ref('SensorData');

dbRef.once("value").then(function(snapshot){
  const datab = snapshot.val();
  console.log("Fire: ", datab.FIRE);
  console.log("LPG: ", datab.LPG);
  console.log("Monoxide: ", datab.Monoxide);
  console.log("Temp: ", datab.Temperature);
  console.log("timehour: ", datab.timehour);
});
console.log("Successful");

export default {
  name: 'Services',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  body{
    background: #262a2e;
  }

  .intro{
    color: #bb86fc;
    font-family: kanit;
  }
</style>
