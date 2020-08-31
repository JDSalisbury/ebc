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
          text: '1227 Hawthorne Ave.<br>Columbus, Ohio 43203',
        },
        {
          icon: 'mdi-cellphone',
          title: 'Phone',
          text: '614.400.4356',
        },
        {
          icon: 'mdi-email',
          title: 'Email',
          text: 'contact@elementalblockchain.com',
        },
      ],
    }),
  }
</script>
