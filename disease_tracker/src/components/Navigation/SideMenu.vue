<template>
  
      <v-navigation-drawer
          v-model="drawer"
          :color="color"
          :expand-on-hover="expandOnHover"
          :mini-variant="miniVariant"
          absolute
          dark
        >
          <v-list
            dense
            nav
            class="py-0"
          >
            <!-- <v-list-item two-line :class="miniVariant && 'px-0'">
              <v-list-item-content>
                <v-list-item-title>Application</v-list-item-title>
                <v-list-item-subtitle>Subtext</v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
  
            <v-divider></v-divider> -->
  
            <v-list-item
              v-for="item in items"
              :key="item.title"
              link
              class="pt-2"
            >
              <v-list-item-icon>
                <v-icon>{{ item.icon }}</v-icon>
              </v-list-item-icon>
  
              <v-list-item-content>
                <v-list-item-title>{{ item.title }}</v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list>
        </v-navigation-drawer>
  
</template>

<script>
export default {
    name: "PiSideMenu",
    data () {
    return {
      drawer: true,
      items: [
        { title: 'Dashboard', icon: 'mdi-view-dashboard' },
        { title: 'Statistics', icon: 'mdi-chart-line' },
        { title: 'News', icon: 'mdi-newspaper-variant' },
      ],
      color: 'primary',
      colors: [
        'primary',
        'blue',
        'success',
        'red',
        'teal',
      ],
      miniVariant: true,
      expandOnHover: true,
      background: false,
    }
    }
}
</script>

<style>

</style>