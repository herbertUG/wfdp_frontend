<template>
  <div class="dashboard">
    <h1 class="subheading grey--text ma-3">Dashboard</h1>
    <v-container class="my-5">
      <v-layout row wrap>
        <v-flex xs12 sm6 md4 lg3 v-for="detail in details" :key="detail.name">
          <v-card flat class="text-xs-center ma-3">
            <v-card-text :class="`${detail.status}`">
              <div class="grey--text display-3">{{detail.count}}</div>
              <div class="subheading">{{detail.name}}</div>
            </v-card-text>
          </v-card>
        </v-flex>
        <v-flex xs12 class="ma-3">
    <v-data-table
        :titles="titles"
    :items="Type"
    class="elevation-1">
      
    </v-data-table>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>
<script>
export default {
  data() {
    return {
      details: [
        {
          name: "Total",
          count: 500
        },
        {
          name: "Approved",
          count: 255
        },
        {
          name: "Waiting",
          count: 78
        },
        {
          name: "My cards",
          count: 300
        }
      ],
    };
  }
};
</script>
<style>
.total {
  background: #1da746;
}
.approved {
  background: #3cd1c2;
}
.waiting {
  background: #ffaa2c;
}
.mycards {
  background: #f83e70;
}
.title:nth-child(1n) {
  margin-right: 68px;
}

</style>
