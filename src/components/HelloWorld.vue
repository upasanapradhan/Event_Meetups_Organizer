<template>
  <v-container>
    <v-row class="text-center">
      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Create Events
        </h1>

        <p class="subheading font-weight-regular">
          For creating and managing events.
        </p>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          Create your own event.
          <br/>
          View upcoming events.
          <br/>
        </h2>
         <v-layout row wrap>
            <v-flex xs12 sm6 class="text-xs-center text-sm-right">
              <v-btn large router to="/meetups" class="info">Explore Meetups</v-btn>
            </v-flex>
            <v-flex xs12 sm6 class="text-xs-center text-sm-left">
              <v-btn large router to="/meetup/new" class="info">Organize Meetup</v-btn>
            </v-flex>
          </v-layout>
        <h2 class="headline font-weight-bold mb-3">
          <br/>
          Links to events
        </h2>
        <v-row justify="center">
          <a
            v-for="(link, i) in importantLinks"
            :key="i"
            :href="link.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ link.text }}
          </a>
        </v-row>
      </v-col>

      <v-col
        class="mb-5"
        cols="12"
      >
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'HelloWorld',

  data: () => ({
    importantLinks: [
      {
        text: 'Google DevFest',
        href: 'https://devfest.withgoogle.com/'
      },
      {
        text: 'WTM Breakfast',
        href: 'https://www.facebook.com/watch/?v=598598720909575'
      },
      {
        text: 'Hackfest kathmandu',
        href: 'https://hackfestktm.github.io/'
      }
    ]
  })
}
</script>
