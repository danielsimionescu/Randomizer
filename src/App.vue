<template>
  <v-app>
    <Toolbar/>
    <Home/>
  </v-app>
</template>

<script>
import Toolbar from "./components/Toolbar";
import Home from "./components/Home";

export default {
  name: "App",
  components: {
    Toolbar,
    Home
  }
};
</script>
