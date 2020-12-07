<template>
  <v-app>
    <Arama/>
    <Navbar/>
    <v-main>
      <v-container>
        <nuxt/>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
  import Arama from "../components/default/Arama";
  import Navbar from "../components/default/Ayakkabiturleri";

  export default {
    components: {Navbar, Arama},
  }
</script>

<style>
  a {
    text-decoration: none;
  }
</style>
