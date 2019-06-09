<template>
  <v-app class="grey lighten-4">
    <Nav />
    <v-content class="mx-4 mb-4">
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
import Nav from "@/components/shared/Nav";
export default {
  components: { Nav },
  name: "App",
  data() {
    return {
      //
    };
  }
};
</script>