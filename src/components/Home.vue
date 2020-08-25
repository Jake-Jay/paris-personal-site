<template>
  <div>
    <v-row class="text-center" style="height:100vh">
      <v-col cols="12">
        <v-img
          :src="require('../assets/paris-bee.svg')"
          contain
          height="320"
          transition="scale-transition"
          class="pa-8"
        />
        <h1 class="pa-8" >PARIS PENCHARZ</h1>

        <v-btn icon class="order">
          <v-icon
            large
            color="black"
            @click="$vuetify.goTo('#about')"
          >mdi-arrow-down</v-icon>
        </v-btn>
      </v-col>
    </v-row>
    <div class="gradient" id="about" style="height:100vh">
      <div class="ma-4 ">
        <h3 class="text-center pb-4">About Paris</h3>
        <p class="text-center">
          Paris is a very lovely person. <br> 
          As a future employer/supervisor this is really all that you need to know. <br> <br>

          She cares deeply about those around her - even if she does not always show it. <br>
          She also cares very deeply about her Shnauzers, and about the cows and sheep and goats and chickens that everyone else eats. <br>
          She cares about the planet, and I think we should be glad that she does. <br>
          Because along with her curly locks, which you can only make out just above the steering wheel, she was born with a very powerful mind. <br>
          So we should all be greatful that she has chosen to use that superpower to help the cows and sheep and goats and chickens. <br>
          And the forests, grasslands, glaciers and mangroves. <br>
          And the bees, butterflies, grasshoppers and spiders. <br>
          And probably many more things which you and I shall never know about. <br><br>

          But what I am the most grateful for, is that she cares about me. <br>
          Because I care about her. <br>
          Very much. <br>
          She is after all, a very lovely person.

        </p>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-family:'Paris-font'; 
  font-size:6rem
}
h3 {
  font-family:'Paris-font'; 
  font-size:3rem
}
p {
  font-family:'Paris-font'; 
  font-size:1.5rem
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
.gradient { 
  background-color: #fbf27e;
  background-image: linear-gradient(62deg, #fbf27e 0%, #F7CE68 100%);
}
.order {
  top: 20vh;
  width: 75px;
  line-height: 75px;
  text-align:center;
  opacity: 1;
  background: #fbf27e;
  color:#fff;
  border-radius:50%;
  -webkit-animation: bounce .3s infinite alternate;
  -moz-animation: bounce .3s infinite alternate;
  animation: bounce .3s infinite alternate;
}
@-webkit-keyframes bounce {
  to { -webkit-transform: scale(1.2); }
}
@-moz-keyframes bounce {
  to { -moz-transform: scale(1.2); }
}
@keyframes bounce {
  to { transform: scale(1.2); }
}
</style>

