<template>
  <v-app id="inspire" >
    <v-navigation-drawer
        v-model="drawer"
        app
        class ="deep-purple lighten-1"
    >
      <v-layout column align-center>
        <v-flex class="mt-5">
          <v-avatar size="100">
            <img src="/profile1.jpg" alt="">
          </v-avatar>
          <p class=" mt-2 ">
            Username </p>
        </v-flex>
      </v-layout>
      <v-list-item  >
        <v-list-item-content  >
          <v-list-item-title class="text-h6">

          </v-list-item-title>
          <v-list-item-subtitle>

          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list
          dense
          nav
      >
        <v-list-item
            v-for="item in items"
            :key="item.title"
            :to = "item.to"
            link
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <!--  -->
    </v-navigation-drawer>

    <v-app-bar app class="deep-purple lighten-1">
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>EZLabor</v-toolbar-title>
    </v-app-bar>

    <v-main>
      <!--  -->
      <router-view></router-view>
    </v-main>

  </v-app>
</template>

<script>
export default {
  name: "navigation-bar",
  data: () => ({
    drawer: null,
    items: [
      { title: 'Home', icon: 'mdi-view-dashboard', to: '/dashboard' },
      { title: 'Explore', icon: 'mdi-briefcase-search', to: '/explore' },
      { title: 'Notifications', icon: 'mdi-bell-badge', to: '/notifications' },
      { title: 'Messages', icon: 'mdi-forum', to: '/messages' },
      { title: 'Offers', icon: 'mdi-briefcase', to: '/offers' },
      { title: 'Profile', icon: 'mdi-account', to: '/profile' },
      { title: 'Meetings', icon: 'mdi-account-multiple-plus', to: '/meetings' },
    ],
    icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-linkedin',
      'mdi-instagram',
    ],
  }),
  methods:{
  }
}
</script>

<style scoped>
</style>
