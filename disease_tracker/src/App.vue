<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Pandemic Insight"
          contain
          src="./assets/PandemicInsightLogo_LogoMaker.png"
          transition="scale-transition"
          width="250"
        />

        <!-- <h2>Pandemic Hub</h2> -->
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-content>
      <pi-side-menu/>
      <v-card
        class="mx-auto"
        width="100%"
        >
      <v-img
        src="./assets/VirusImg.png"
        class="m-2"
        style="width:100%;"
      />
      </v-card>
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import PiSideMenu from './components/Navigation/SideMenu';

export default {
  name: 'App',
  components: {
    HelloWorld,
    PiSideMenu
  },

  data: () => ({
    //
  }),
};
</script>
