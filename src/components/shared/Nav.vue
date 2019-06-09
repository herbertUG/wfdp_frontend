<template>
  <nav>
    <v-toolbar
      color="blue darken-3"
      dark
      app
      fixed
    >
      <v-toolbar-title
        style="width: 250px"
        class="ml-0 pl-3"
      >
        <!-- <v-toolbar-side-icon @click.stop="drawer = !drawer"></v-toolbar-side-icon> -->
        <span class="hidden-sm-and-down">WFDP</span>
      </v-toolbar-title>
      <v-text-field
        flat
        solo-inverted
        hide-details
        prepend-inner-icon="search"
        label="Search"
        class="hidden-sm-and-down"
      ></v-text-field>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>apps</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>notifications</v-icon>
      </v-btn>
      <v-btn
        icon
        large
      >
        <v-icon>account_circle</v-icon>
      </v-btn>
      <v-btn
        flat
        color="grey"
        router
        to="/login"
      >
        <span>Sign Out</span>
        <v-icon right>exit_to_app</v-icon>
      </v-btn>
    </v-toolbar>

    <SideBar />
  </nav>
</template>

<script>
import SideBar from "./SideBar";
export default {
  components: {
    SideBar
  }
};
</script>