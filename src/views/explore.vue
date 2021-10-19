<template>
  <v-flex>
    <appbar/>
    <Navbar/>
  </v-flex>
</template>

<script>
import appbar from "../components/appbar";
import Navbar from "../components/Navbar";
export default {
  name: "explore",
  components:{
    appbar,
    Navbar,
  }
}
</script>

<style scoped>

</style>