<template>
  <v-data-table
    :headers="headers"
    :items="details"
    class="elevation-1"
    disable-initial-sort
    hide-actions
    light
  >
    <template v-slot:items="props">
      <td>{{ props.item.type }}</td>
      <td>{{ props.item.surname, }}</td>
      <td>{{ props.item.givenName }}</td>
      <td>{{ props.item.title }}</td>
      <td>{{ props.item.nationality }}</td>
      <td>{{ props.item.sex }}</td>
      <td>{{ props.item.organisation }}</td>
      <td>{{ props.item.dateOfBirth }}</td>
      <td>{{ props.item.dateOfIssue }}</td>
      <td>{{ props.item.dateOfExpiry }}</td>
      <td>{{ props.item.placeOfBirth }}</td>
      <td>{{ props.item.signature }}</td>
    </template>
  </v-data-table>
</template>

<script>
export default {
  data() {
    return {
      headers: [
        {
          text: "Type",
          value: "type"
        },
        {
          text: "Surname",
          value: "surname"
        },
        {
          text: "Givename",
          value: "givenName"
        },

        {
          text: "Title",
          value: "title"
        },
        {
          text: "Nationality",
          value: "nationality"
        },
        {
          text: "Sex",
          value: "sex"
        },
        {
          text: "Organisation",
          value: "organisation"
        },
        {
          text: "D.O.B",
          value: "dateOfBirth"
        },
        {
          text: "D.O.I",
          value: "dateOfIssue"
        },
        {
          text: "D.O.E",
          value: "dateOfExpiry"
        },
        {
          text: "P.O.B",
          value: "placeOfBirth"
        },
        {
          text: "Signature",
          value: "signature"
        }
      ],
      details: [
        {
          type: "P",
          surname: "name1",
          givenName: "name2",
          nationality: "nationality",
          dateOfBirth: "dateOfBirth",
          dateOfIssue: "dateOfIssue",
          placeOfBirth: "placeOfBirth",
          dateOfExpiry: "dateOfExpiry",
          title: "title",
          sex: "sex",
          organisation: "organisation",
          signature: "signature"
        }
      ]
    };
  }
};
</script>