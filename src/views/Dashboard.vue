<template>
  <div class="dashboard">
    <v-layout
      class="ml-5 mt-3"
      row
      wrap
    >
      <v-flex
        v-for="detail in details"
        :key="detail.name"
      >
        <v-card
          flat
          class="text-xs-center"
          id="cardStyle"
        >
          <v-card-text :class="`${detail.status}`">
            <div class="display-3">{{detail.count}}</div>
            <div class="subheading">{{detail.name}}</div>
          </v-card-text>
        </v-card>
      </v-flex>
      <v-flex
        xs12
        class="ma-3"
      >
      </v-flex>
    </v-layout>
    <Table class="ml-5" />
  </div>
</template>
<script>
import Table from "../components/shared/Table";
export default {
  components: {
    Table
  },
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
        },
        {
          name: "My cards",
          count: 300
        }
      ]
    };
  }
};
</script>
<style>
#cardStyle {
  box-shadow: 0 4px 9px 0 rgba(0, 0, 0, 0.1);
  background-color: #ffffff;
  border-radius: 6px;
  width: 350px;
}
.total {
  color: aqua;
}
.cards {
  color: blueviolet;
}
</style>
