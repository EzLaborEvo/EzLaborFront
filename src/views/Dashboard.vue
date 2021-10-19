<template>
  <v-app>
    <v-flex>
      <v-card class="mb-6">

      </v-card>
      <v-layout row wrap>

        <v-container grid-list-xl>
          <v-layout column>

            <offers-dashboard></offers-dashboard>
            <offers-dashboard></offers-dashboard>
            <offers-dashboard></offers-dashboard>
            <offers-dashboard></offers-dashboard>



          </v-layout>
        </v-container>
      </v-layout>
    </v-flex>
    <navigation-bar></navigation-bar>


  </v-app>

</template>

<script>
import appbar from "../components/appbar";
import Navbar from "../components/Navbar";
import OffersDashboard from "../components/offers-dashboard";
import NavigationBar from "../components/navigation-bar";
export default {
  name: "Dashboard.vue",
  components:{
    NavigationBar,
    OffersDashboard,
    appbar,
    Navbar,

  }
}
</script>

<style scoped>
  v-btn {
    position: absolute;
    width: 141px;
    height: 49px;
    left: 23px;
    top: 283px;
  }
</style>
