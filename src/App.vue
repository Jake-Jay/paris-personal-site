<template>
  <v-app>
    <v-app-bar
      app
      color="white"
      elevate-on-scroll
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src='./assets/paris-bee.png'
          transition="scale-transition"
          width="40"
        />
      </div>
      <v-spacer></v-spacer>
      <a href="/documents/Paris Pencharz 2020 CV.pdf" download>
        <v-btn text >CV</v-btn>
      </a>
      <a href="/documents/birthdays.pdf" download>
        <v-btn text >Research</v-btn> 
      </a>

      
    </v-app-bar>

    <v-main>
      <Home/>
    </v-main>
  </v-app>
</template>

<script>
import Home from './components/Home';

export default {
  name: 'App',

  components: {
    Home,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
@font-face {
  font-family: "Paris-font";
  src: local("Paris-font"),
   url(./fonts/Evolution-Regular.ttf) format("truetype");
}

a {
  text-decoration: none;
}
</style>

