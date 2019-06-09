<template>
  <v-data-table
    :headers="headers"
    :items="details"
    class="elevation-1"
    id="table"
    disable-initial-sort
    hide-actions
    light
  >
    <template v-slot:items="props">
      <td>{{ props.item.type }}</td>
      <td>{{ props.item.surname, }}</td>
      <td>{{ props.item.givenName }}</td>
      <td>{{ props.item.nationality }}</td>
      <td>{{ props.item.sex }}</td>
      <td>{{ props.item.organisation }}</td>
      <td>{{ props.item.dateOfBirth }}</td>
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
          value: "type",
          sortable: true
        },
        {
          text: "Surname",
          value: "surname",
          sortable: false
        },
        {
          text: "Givename",
          value: "givenName",
          sortable: false
        },

        {
          text: "Nationality",
          value: "nationality",
          sortable: false
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
          value: "dateOfBirth",
          sortable: false
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
        },
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
        },
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
        },
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
        },
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
        },
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
        },
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
        },
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
        },
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
        },
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
        },
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
        },
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
