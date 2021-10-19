<template>
  <v-flex>
    <uwu/>
    <appbar/>
    <Navbar/>
  </v-flex>
</template>

<script>
import appbar from "../components/appbar";
import Navbar from "../components/Navbar";
import uwu from "../components/nuevo1/uwu";
export default {
  name: "messages",
  components:{
    appbar,
    Navbar,
    uwu,
  }
}
</script>

<style scoped>

</style>
