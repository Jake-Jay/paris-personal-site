<template>
  <div>
    <v-row class="text-center" style="height:100vh">
      <v-col cols="12">
        <v-img
          :src="require('../assets/paris-bee.svg')"
          contain
          height="320"
          transition="scale-transition"
          class="pa-8 img_hover"
        />
        <h1 class="pa-8" >PARIS PENCHARZ</h1>

        <button icon class="order">
          <v-icon
            large
            color="black"
            @click="$vuetify.goTo('#about')"
          >mdi-arrow-down</v-icon>
        </button>
      </v-col>
    </v-row>
    <div class="gradient" id="about" >
      <div class="ma-4 ">
        <h3 class="text-center pb-4">About Paris</h3>
        <p class="text-center py-4">
          Paris is a very lovely person. <br> 
          As a future employer/supervisor this is really all that you need to know. <br> <br>

          She cares deeply about those around her - even if she does not always show it. <br>
          She also cares very deeply about her Shnauzers, and about the cows and sheep and goats and chickens that everyone else eats. <br>
          She cares about the planet, and I think we should be glad that she does. <br>
          Because along with her curly locks, which you can only make out just above the steering wheel, she was born with a very powerful mind. <br>
          So we should all be greatful that she has chosen to use that superpower to help the cows and sheep and goats and chickens. <br>
          And the forests, grasslands, glaciers and mangroves. <br>
          And the bees, butterflies, grasshoppers and spiders. <br>
          And probably many more things which you and I shall never know about. 
        </p>
        <v-img
          :src="require('../assets/earth.svg')"
          contain
          height="320"
          transition="scale-transition"
          class="py-8"
        />
        <p class="text-center pa-8">
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
  position: absolute;
  top: 75vh;
  width: 50px;
  line-height: 50px;
  margin-left: -25px;
  opacity: 1;
  background: #fbf27e;
  border-radius:50%;
  -webkit-animation: bounce .8s infinite alternate;
  -moz-animation: bounce .8s infinite alternate;
  animation: bounce .8s infinite alternate;
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
.img_hover:hover {
  /* Start the shake animation and make the animation last for 0.5 seconds */
  animation: shake 0.5s;

  /* When the animation is finished, start again */
  animation-iteration-count: infinite;
}

@keyframes shake {
  0% { transform: translate(1px, 1px) rotate(0deg); }
  10% { transform: translate(-1px, -2px) rotate(-1deg); }
  20% { transform: translate(-3px, 0px) rotate(1deg); }
  30% { transform: translate(3px, 2px) rotate(0deg); }
  40% { transform: translate(1px, -1px) rotate(1deg); }
  50% { transform: translate(-1px, 2px) rotate(-1deg); }
  60% { transform: translate(-3px, 1px) rotate(0deg); }
  70% { transform: translate(3px, 1px) rotate(-1deg); }
  80% { transform: translate(-1px, -1px) rotate(1deg); }
  90% { transform: translate(1px, 2px) rotate(0deg); }
  100% { transform: translate(1px, -2px) rotate(-1deg); }
}
</style>

