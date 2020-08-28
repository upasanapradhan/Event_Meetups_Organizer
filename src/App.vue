<template>
  <v-app>
    <v-app-bar
      absolute
      color="primary"
      dark
      shrink-on-scroll
      prominent
      scroll-target="#scrolling-techniques"
    >
    <v-app-bar-nav-icon></v-app-bar-nav-icon>
    <v-toolbar-title>LET'S MEETUP</v-toolbar-title>
    <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
       <v-btn icon>
        <v-icon>mdi-export</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <HelloWorld/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',

  components: {
    HelloWorld
  },

  data: () => ({
    //
  })
}
</script>
