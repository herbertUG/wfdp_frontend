<template>
  <v-navigation-drawer
    :clipped="true"
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
</template>

<script>
export default {
  data() {
    return {
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
