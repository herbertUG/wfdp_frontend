<template>
  <nav>
    <v-toolbar
      color="blue darken-3"
      dark
      app
      fixed
    >
      <v-toolbar-title
        style="width: 300px"
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

    <v-navigation-drawer
      :clipped="$vuetify.breakpoint.lgAndUp"
      fixed
      app
    >
      <v-list
        dense
        align-center
      >
        <v-list-tile
          v-for="link in links"
          :key="link.text"
          router
          :to="link.route"
        >
          <v-list-tile-action>
            <v-icon>{{ link.icon }}</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>{{ link.text }}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      drawer: true,
      links: [
        { icon: "dashboard", text: "Dashboard", route: "/" },
        { icon: "add_box", text: "Create Card", route: "/newCard" },
        { icon: "folder", text: "My Cards", route: "/Cards" },
        { icon: "person", text: "Profile", route: "/userProfile" }
      ]
    };
  }
};
</script>