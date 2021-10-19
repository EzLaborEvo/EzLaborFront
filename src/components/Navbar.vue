<template>
  <v-navigation-drawer>
    <v-layout mt-4 column align-center>
      <v-flex>
        <v-avatar>
          <img src="https://cdn-icons-png.flaticon.com/512/2550/2550359.png" alt="">
        </v-avatar>
      </v-flex>
      <v-flex>
        <p class="black--text mt-3 headline"> New User </p>
      </v-flex>
    </v-layout>
    <v-layout column>
      <v-flex mx-03>
        <v-btn color=#7146ed class="white--text mb-3" block :to="{name: 'dashboard'}" > Home</v-btn>
        <v-btn color=#E4DAFF class="black--text mb-3" block :to="{name: 'explore'}"> Explore </v-btn>
        <v-btn color=#E4DAFF class="black--text mb-3" block :to="{name: 'notifications'}"> Notifications </v-btn>
        <v-btn color=#E4DAFF class="black--text mb-3" block :to="{name: 'messages'}"> Messages </v-btn>
        <v-btn color=#E4DAFF class="black--text mb-3" block :to="{name: 'offers'}"> Offers </v-btn>
        <v-btn color=#E4DAFF class="black--text mb-3"  block :to="{name: 'profile'}"> Profile </v-btn>
        <v-btn color=#E4DAFF class="black--text mb-3" block :to="{name: 'meetings'}"> Meetings </v-btn>
      </v-flex>
    </v-layout>
  </v-navigation-drawer>
</template>

<script>
export default {
  name: "Navbar"
}
</script>

<style scoped>

</style>