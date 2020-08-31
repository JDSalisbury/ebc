<template>
  <v-theme-provider :dark="dark">
    <div>
      <base-title
        size="body-1"
        space="4"
        title="About Elemental Blockchain"
        weight="regular"
      />

      <base-body>
        "We create Synergies between energy producers and crypto miners by leveraging behind the meter energy prices that other miners can't replicate."
      </base-body>
    </div>
  </v-theme-provider>
</template>

<script>
  export default {
    name: 'BaseInfo',

    props: {
      title: String,
      dark: Boolean,
    },

    data: () => ({
      business: [
        {
          icon: 'mdi-map-marker-outline',
          title: 'Address',
          text: '8553 N. Beach St. Ste. 227<br>Fort Worth, Texas 76137',
        },
        {
          icon: 'mdi-cellphone',
          title: 'Phone',
          text: '01 (800) 433 744<br>01 (800) 433 633',
        },
        {
          icon: 'mdi-email',
          title: 'Email',
          text: 'john@vuetifyjs.com<br>heather@vuetifyjs.com',
        },
      ],
    }),
  }
</script>
