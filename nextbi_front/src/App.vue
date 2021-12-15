<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <v-app-bar-nav-icon @click="drawer = !drawer" />
      
      <v-toolbar-title>Page title</v-toolbar-title>
      <v-app-bar-title>Title</v-app-bar-title>

      <v-spacer />
    </v-app-bar>
    
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <v-main>
        <HelloWorld />
      </v-main>
    </v-navigation-drawer>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    drawer: false
    //
  }),
};
</script>
