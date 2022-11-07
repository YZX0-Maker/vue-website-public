<template>
  <v-app>
    <v-app-bar app color="white">
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <div ><v-btn href="/" text>Yean</v-btn></div>
      </div>

      <v-spacer></v-spacer>
      <v-btn class="hidden-mobile"
        href=""
        target="_blank"
        text
      >
        <span class="mr-2">Linkedin</span>
        <v-icon>mdi-linkedin</v-icon>
      </v-btn>
      <v-btn class="hidden-mobile"
        href=""
        target="_blank"
        text
      >
        <span class="mr-2">Github</span>
        <v-icon>mdi-github</v-icon>
      </v-btn>
      <v-btn 
        href="/projects"
        text
      >
        <span class="mr-2">Projects</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>
<style>
  @import "assets/css/Treegarden.css";
</style>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
